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
-	[`nats:2.10.2`](#nats2102)
-	[`nats:2.10.2-alpine`](#nats2102-alpine)
-	[`nats:2.10.2-alpine3.18`](#nats2102-alpine318)
-	[`nats:2.10.2-linux`](#nats2102-linux)
-	[`nats:2.10.2-nanoserver`](#nats2102-nanoserver)
-	[`nats:2.10.2-nanoserver-1809`](#nats2102-nanoserver-1809)
-	[`nats:2.10.2-scratch`](#nats2102-scratch)
-	[`nats:2.10.2-windowsservercore`](#nats2102-windowsservercore)
-	[`nats:2.10.2-windowsservercore-1809`](#nats2102-windowsservercore-1809)
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
$ docker pull nats@sha256:00950ae452fd32e036bb1de4eca8cb02902ad876425626cf4b752f44057e4b06
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
	-	windows version 10.0.17763.4974; amd64

### `nats:2` - linux; amd64

```console
$ docker pull nats@sha256:7be2e854c9542ad2146d9baadede0f2e3d520d9ffc8b9ef24078852362d95c5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5469432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d633df072e1a202141ac94a984750c13337fede7f772b34400dc99a9285cd99`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:a7de81fdc98e0908f1fbfd4b16f2eeac146932aac03b4a109a89f93b3efbfc58 in /nats-server 
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:20:31 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:20:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:20:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:494ad87960e9c491e7d14b1b9a5ca82020e4b968c60a0f3bffece88c8cee4831`  
		Last Modified: Sun, 08 Oct 2023 12:45:05 GMT  
		Size: 5.5 MB (5468923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d4a6b4c3024603d5932b75b727d2b94f22a490f5326099a6112bf261dfebc5`  
		Last Modified: Mon, 09 Oct 2023 23:21:26 GMT  
		Size: 509.0 B  
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
$ docker pull nats@sha256:4311525539cb532e2215a0f0e6a97e456bf100aecae9df633068dce84725d3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5189188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b74620a2c8b938dece7aba41cf3db596039ac4579268f2083d879dc0338e3d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:78bf14fdba87d3f994b59ec64fa5f813ff988f0f91e4929c7aaf33d206d6e4e2 in /nats-server 
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:49:30 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:49:30 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:49:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:541bfb4a7866a6fb7234b9fb133b37cc8a1fff7bcf10779570793f66bfa36cc5`  
		Last Modified: Mon, 09 Oct 2023 23:50:25 GMT  
		Size: 5.2 MB (5188681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e9969a228338f491f74c367e86a77a512ae318604d924fa624ef4e9b944a62`  
		Last Modified: Mon, 09 Oct 2023 23:50:24 GMT  
		Size: 507.0 B  
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
$ docker pull nats@sha256:72a048e9abb13148a5588dd1f556af5cf11e91369fd856d21e1b981e2f0f6aec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3f7200638809e9d2ec5971ab53b5a84b4413d7fce360c58f1d7381d739555e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:dfba40eb121bd5821909fe10c59b498aec418c7224d18a7961e71444dc375765 in /nats-server 
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:57:51 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c24b02c85cdfcd5bdce9a848ef068ff9e9535a6287fb7a00eb8e39b357c54ad0`  
		Last Modified: Mon, 09 Oct 2023 23:58:40 GMT  
		Size: 5.2 MB (5177978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d844de696d0e40f4aff106f51467e397619526062047fe60f4b692adda3bd736`  
		Last Modified: Mon, 09 Oct 2023 23:58:39 GMT  
		Size: 507.0 B  
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
$ docker pull nats@sha256:4b167dea0c683971c7d06db669fbdebf2a8b3c01cb4d229bf5204c8fc6cab7e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5042145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966bdbd5f41b922365e541cf6121d6cf76a4ddb1f9c111e010656f7041d50c1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:c0f257aca3b8b7405bb5549a368de7ae62c806fe4e75e189b405a7ce1f65fa4b in /nats-server 
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:39:55 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:39:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:39:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12032ad6ebd443b7c142112d1df3d64b3deb3a403e0a99764593e5fe7843781b`  
		Last Modified: Mon, 09 Oct 2023 23:40:46 GMT  
		Size: 5.0 MB (5041638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7d34c174da06f5ab9c869a0197e492849a0d80fbf8f038f93e9e1ac634d1f7`  
		Last Modified: Mon, 09 Oct 2023 23:40:45 GMT  
		Size: 507.0 B  
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

### `nats:2` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:d0a9a23bc5e727b8b8db67f5a02c6be5d0dfba5700152d11e56457862713e866
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110053852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f669b1f92bc1e89b2470de199627f90a4496308a2cd8c5f8bfd06b52ecf39a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:36:34 GMT
RUN cmd /S /C #(nop) COPY file:56de93ec6afaefd5f19b9effd4409842fdfa695280fb05da230b1d12a03db7bb in C:\nats-server.exe 
# Wed, 11 Oct 2023 03:36:35 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52fe086e7510cd640f31a862cc7ed0aae171d6591241c4eddfbeda3169a718b`  
		Last Modified: Wed, 11 Oct 2023 03:40:51 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f15b99379f9a65c4a40e86d7f09407cf716ae5cdd5ec3fdfbcd609fceb69f5`  
		Last Modified: Wed, 11 Oct 2023 03:40:50 GMT  
		Size: 5.6 MB (5582847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3574203dd8b3d01c5d1979302e56d73e3c604318c215efb12f98e667c80879`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937e84807bea241751a5e003bbf2cca02d1a37306e3cd7d17e260322cebb9e70`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fde0249533da9dfa2f6b077b43c2290316223ac025f271a8ba383f1136ff00`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee3b7476b8b4cb6aa82268271e5e2971d380d8da227366182b80abcfacc961`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine`

```console
$ docker pull nats@sha256:c6d778a0df2aeeec2399f1e1ce558d7b65e70adc7ef5ca13f2cf06b1f7654a08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:d6a47f89f52342be07d213d493e0b71a80fc94ccc19edc9c8b17169e8d887fbe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9494811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18e20b07c9925b57a0846b64bffdab236ff0d02728bea2661094cb2f1088d89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:20:15 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:20:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:20:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:20:17 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:20:17 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:20:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:20:17 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793ee3203ddeae4265feedfeeb0176c5d046487786e6430ec414b466b7342687`  
		Last Modified: Mon, 09 Oct 2023 23:21:01 GMT  
		Size: 6.1 MB (6091846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0dd902fefeb39726cbb9025e935fabe591af4d39f448ddad514c70eb56a6002`  
		Last Modified: Mon, 09 Oct 2023 23:21:00 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7a1bcf5bcb5ad0317a82f43795966d7b0cf297054e112bc548fe8d0c881df9`  
		Last Modified: Mon, 09 Oct 2023 23:21:00 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:6d9d5fd5f91a7c3e45e2cac23df6f50393e2024ea69495d9233df8ba9503bdc8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8958058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11708ece1d9ad1b7baf64c1f3c5e3b7a38ef5d66e87c24ba859eb6272bc2694f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:49:18 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:49:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:49:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:49:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:49:21 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dece2e91316626c2aeb73fab796c9095ba11a38f43e17e03f3cea33bada9941e`  
		Last Modified: Mon, 09 Oct 2023 23:49:58 GMT  
		Size: 5.8 MB (5811761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0164ce1b0fe0ce335f0348dbf1ef83dca670a9bb6c3036586e38f45c257ab3`  
		Last Modified: Mon, 09 Oct 2023 23:49:57 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a6185289b767b3266aeff451a57e88263f01cbb1544b137dd118ad2aa87d88`  
		Last Modified: Mon, 09 Oct 2023 23:49:57 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:56973c518df167ff13997d599dd6f0f488eb2a00380d161395d001cbd82ef4f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8701812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c71794277a3ea4fd3358f79bd24730e7bff545f116dbae54391ff86f7b5ba91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:57:29 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:57:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:57:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:57:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:57:31 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:57:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1577c013973725bb512b6e87006f323da7dece18dc8d5cddf516ac8ac1bd3690`  
		Last Modified: Mon, 09 Oct 2023 23:58:15 GMT  
		Size: 5.8 MB (5800912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2989475d4fcb37e49592f48904864c46ac84f25ca502bbddacc54bddf27ec9a3`  
		Last Modified: Mon, 09 Oct 2023 23:58:14 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dca18857ae02bbc23b7a6d389a1036fd7822d30861d1f065a1fce1b2662745e`  
		Last Modified: Mon, 09 Oct 2023 23:58:14 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a1cc118cb20105a3d28409f6f0134779e37d691cdfc8340e26aa21bf5c1fcecb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8999244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c690558bd2217d60e3ef1f45a02405b0c52118f1c91dda8b42c091696af68306`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:39:44 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:39:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:39:47 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:39:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e016e40994857a38606186dc8f2061ac54ed621273f59128aa5c6d060fb22`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 5.7 MB (5666417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15cff88ae624a30801728dd1b20bb84f6e871846c236cf2613ec7c7fb6008f1`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68049c030ad10066e6a3a63f9d02398f98a4b8bf2104c8d22adb9aed0ff83e1`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-alpine3.18`

```console
$ docker pull nats@sha256:c6d778a0df2aeeec2399f1e1ce558d7b65e70adc7ef5ca13f2cf06b1f7654a08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:d6a47f89f52342be07d213d493e0b71a80fc94ccc19edc9c8b17169e8d887fbe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9494811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18e20b07c9925b57a0846b64bffdab236ff0d02728bea2661094cb2f1088d89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:20:15 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:20:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:20:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:20:17 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:20:17 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:20:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:20:17 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793ee3203ddeae4265feedfeeb0176c5d046487786e6430ec414b466b7342687`  
		Last Modified: Mon, 09 Oct 2023 23:21:01 GMT  
		Size: 6.1 MB (6091846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0dd902fefeb39726cbb9025e935fabe591af4d39f448ddad514c70eb56a6002`  
		Last Modified: Mon, 09 Oct 2023 23:21:00 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7a1bcf5bcb5ad0317a82f43795966d7b0cf297054e112bc548fe8d0c881df9`  
		Last Modified: Mon, 09 Oct 2023 23:21:00 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:6d9d5fd5f91a7c3e45e2cac23df6f50393e2024ea69495d9233df8ba9503bdc8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8958058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11708ece1d9ad1b7baf64c1f3c5e3b7a38ef5d66e87c24ba859eb6272bc2694f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:49:18 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:49:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:49:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:49:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:49:21 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dece2e91316626c2aeb73fab796c9095ba11a38f43e17e03f3cea33bada9941e`  
		Last Modified: Mon, 09 Oct 2023 23:49:58 GMT  
		Size: 5.8 MB (5811761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0164ce1b0fe0ce335f0348dbf1ef83dca670a9bb6c3036586e38f45c257ab3`  
		Last Modified: Mon, 09 Oct 2023 23:49:57 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a6185289b767b3266aeff451a57e88263f01cbb1544b137dd118ad2aa87d88`  
		Last Modified: Mon, 09 Oct 2023 23:49:57 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:56973c518df167ff13997d599dd6f0f488eb2a00380d161395d001cbd82ef4f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8701812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c71794277a3ea4fd3358f79bd24730e7bff545f116dbae54391ff86f7b5ba91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:57:29 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:57:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:57:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:57:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:57:31 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:57:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1577c013973725bb512b6e87006f323da7dece18dc8d5cddf516ac8ac1bd3690`  
		Last Modified: Mon, 09 Oct 2023 23:58:15 GMT  
		Size: 5.8 MB (5800912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2989475d4fcb37e49592f48904864c46ac84f25ca502bbddacc54bddf27ec9a3`  
		Last Modified: Mon, 09 Oct 2023 23:58:14 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dca18857ae02bbc23b7a6d389a1036fd7822d30861d1f065a1fce1b2662745e`  
		Last Modified: Mon, 09 Oct 2023 23:58:14 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a1cc118cb20105a3d28409f6f0134779e37d691cdfc8340e26aa21bf5c1fcecb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8999244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c690558bd2217d60e3ef1f45a02405b0c52118f1c91dda8b42c091696af68306`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:39:44 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:39:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:39:47 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:39:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e016e40994857a38606186dc8f2061ac54ed621273f59128aa5c6d060fb22`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 5.7 MB (5666417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15cff88ae624a30801728dd1b20bb84f6e871846c236cf2613ec7c7fb6008f1`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68049c030ad10066e6a3a63f9d02398f98a4b8bf2104c8d22adb9aed0ff83e1`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-linux`

```console
$ docker pull nats@sha256:6a7739943a7360813f70dba186b72c6aba2163f2809fce7672cc3657b62043ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:7be2e854c9542ad2146d9baadede0f2e3d520d9ffc8b9ef24078852362d95c5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5469432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d633df072e1a202141ac94a984750c13337fede7f772b34400dc99a9285cd99`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:a7de81fdc98e0908f1fbfd4b16f2eeac146932aac03b4a109a89f93b3efbfc58 in /nats-server 
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:20:31 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:20:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:20:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:494ad87960e9c491e7d14b1b9a5ca82020e4b968c60a0f3bffece88c8cee4831`  
		Last Modified: Sun, 08 Oct 2023 12:45:05 GMT  
		Size: 5.5 MB (5468923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d4a6b4c3024603d5932b75b727d2b94f22a490f5326099a6112bf261dfebc5`  
		Last Modified: Mon, 09 Oct 2023 23:21:26 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:4311525539cb532e2215a0f0e6a97e456bf100aecae9df633068dce84725d3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5189188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b74620a2c8b938dece7aba41cf3db596039ac4579268f2083d879dc0338e3d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:78bf14fdba87d3f994b59ec64fa5f813ff988f0f91e4929c7aaf33d206d6e4e2 in /nats-server 
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:49:30 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:49:30 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:49:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:541bfb4a7866a6fb7234b9fb133b37cc8a1fff7bcf10779570793f66bfa36cc5`  
		Last Modified: Mon, 09 Oct 2023 23:50:25 GMT  
		Size: 5.2 MB (5188681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e9969a228338f491f74c367e86a77a512ae318604d924fa624ef4e9b944a62`  
		Last Modified: Mon, 09 Oct 2023 23:50:24 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:72a048e9abb13148a5588dd1f556af5cf11e91369fd856d21e1b981e2f0f6aec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3f7200638809e9d2ec5971ab53b5a84b4413d7fce360c58f1d7381d739555e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:dfba40eb121bd5821909fe10c59b498aec418c7224d18a7961e71444dc375765 in /nats-server 
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:57:51 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c24b02c85cdfcd5bdce9a848ef068ff9e9535a6287fb7a00eb8e39b357c54ad0`  
		Last Modified: Mon, 09 Oct 2023 23:58:40 GMT  
		Size: 5.2 MB (5177978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d844de696d0e40f4aff106f51467e397619526062047fe60f4b692adda3bd736`  
		Last Modified: Mon, 09 Oct 2023 23:58:39 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:4b167dea0c683971c7d06db669fbdebf2a8b3c01cb4d229bf5204c8fc6cab7e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5042145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966bdbd5f41b922365e541cf6121d6cf76a4ddb1f9c111e010656f7041d50c1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:c0f257aca3b8b7405bb5549a368de7ae62c806fe4e75e189b405a7ce1f65fa4b in /nats-server 
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:39:55 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:39:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:39:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12032ad6ebd443b7c142112d1df3d64b3deb3a403e0a99764593e5fe7843781b`  
		Last Modified: Mon, 09 Oct 2023 23:40:46 GMT  
		Size: 5.0 MB (5041638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7d34c174da06f5ab9c869a0197e492849a0d80fbf8f038f93e9e1ac634d1f7`  
		Last Modified: Mon, 09 Oct 2023 23:40:45 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver`

```console
$ docker pull nats@sha256:d2017f7731ec6420f52e2633c4567934fc67c6b1466820f14cf57a737f77433c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2-nanoserver` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:d0a9a23bc5e727b8b8db67f5a02c6be5d0dfba5700152d11e56457862713e866
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110053852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f669b1f92bc1e89b2470de199627f90a4496308a2cd8c5f8bfd06b52ecf39a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:36:34 GMT
RUN cmd /S /C #(nop) COPY file:56de93ec6afaefd5f19b9effd4409842fdfa695280fb05da230b1d12a03db7bb in C:\nats-server.exe 
# Wed, 11 Oct 2023 03:36:35 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52fe086e7510cd640f31a862cc7ed0aae171d6591241c4eddfbeda3169a718b`  
		Last Modified: Wed, 11 Oct 2023 03:40:51 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f15b99379f9a65c4a40e86d7f09407cf716ae5cdd5ec3fdfbcd609fceb69f5`  
		Last Modified: Wed, 11 Oct 2023 03:40:50 GMT  
		Size: 5.6 MB (5582847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3574203dd8b3d01c5d1979302e56d73e3c604318c215efb12f98e667c80879`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937e84807bea241751a5e003bbf2cca02d1a37306e3cd7d17e260322cebb9e70`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fde0249533da9dfa2f6b077b43c2290316223ac025f271a8ba383f1136ff00`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee3b7476b8b4cb6aa82268271e5e2971d380d8da227366182b80abcfacc961`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:d2017f7731ec6420f52e2633c4567934fc67c6b1466820f14cf57a737f77433c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:d0a9a23bc5e727b8b8db67f5a02c6be5d0dfba5700152d11e56457862713e866
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110053852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f669b1f92bc1e89b2470de199627f90a4496308a2cd8c5f8bfd06b52ecf39a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:36:34 GMT
RUN cmd /S /C #(nop) COPY file:56de93ec6afaefd5f19b9effd4409842fdfa695280fb05da230b1d12a03db7bb in C:\nats-server.exe 
# Wed, 11 Oct 2023 03:36:35 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52fe086e7510cd640f31a862cc7ed0aae171d6591241c4eddfbeda3169a718b`  
		Last Modified: Wed, 11 Oct 2023 03:40:51 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f15b99379f9a65c4a40e86d7f09407cf716ae5cdd5ec3fdfbcd609fceb69f5`  
		Last Modified: Wed, 11 Oct 2023 03:40:50 GMT  
		Size: 5.6 MB (5582847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3574203dd8b3d01c5d1979302e56d73e3c604318c215efb12f98e667c80879`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937e84807bea241751a5e003bbf2cca02d1a37306e3cd7d17e260322cebb9e70`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fde0249533da9dfa2f6b077b43c2290316223ac025f271a8ba383f1136ff00`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee3b7476b8b4cb6aa82268271e5e2971d380d8da227366182b80abcfacc961`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-scratch`

```console
$ docker pull nats@sha256:6a7739943a7360813f70dba186b72c6aba2163f2809fce7672cc3657b62043ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:7be2e854c9542ad2146d9baadede0f2e3d520d9ffc8b9ef24078852362d95c5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5469432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d633df072e1a202141ac94a984750c13337fede7f772b34400dc99a9285cd99`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:a7de81fdc98e0908f1fbfd4b16f2eeac146932aac03b4a109a89f93b3efbfc58 in /nats-server 
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:20:31 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:20:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:20:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:494ad87960e9c491e7d14b1b9a5ca82020e4b968c60a0f3bffece88c8cee4831`  
		Last Modified: Sun, 08 Oct 2023 12:45:05 GMT  
		Size: 5.5 MB (5468923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d4a6b4c3024603d5932b75b727d2b94f22a490f5326099a6112bf261dfebc5`  
		Last Modified: Mon, 09 Oct 2023 23:21:26 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:4311525539cb532e2215a0f0e6a97e456bf100aecae9df633068dce84725d3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5189188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b74620a2c8b938dece7aba41cf3db596039ac4579268f2083d879dc0338e3d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:78bf14fdba87d3f994b59ec64fa5f813ff988f0f91e4929c7aaf33d206d6e4e2 in /nats-server 
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:49:30 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:49:30 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:49:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:541bfb4a7866a6fb7234b9fb133b37cc8a1fff7bcf10779570793f66bfa36cc5`  
		Last Modified: Mon, 09 Oct 2023 23:50:25 GMT  
		Size: 5.2 MB (5188681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e9969a228338f491f74c367e86a77a512ae318604d924fa624ef4e9b944a62`  
		Last Modified: Mon, 09 Oct 2023 23:50:24 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:72a048e9abb13148a5588dd1f556af5cf11e91369fd856d21e1b981e2f0f6aec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3f7200638809e9d2ec5971ab53b5a84b4413d7fce360c58f1d7381d739555e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:dfba40eb121bd5821909fe10c59b498aec418c7224d18a7961e71444dc375765 in /nats-server 
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:57:51 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c24b02c85cdfcd5bdce9a848ef068ff9e9535a6287fb7a00eb8e39b357c54ad0`  
		Last Modified: Mon, 09 Oct 2023 23:58:40 GMT  
		Size: 5.2 MB (5177978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d844de696d0e40f4aff106f51467e397619526062047fe60f4b692adda3bd736`  
		Last Modified: Mon, 09 Oct 2023 23:58:39 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:4b167dea0c683971c7d06db669fbdebf2a8b3c01cb4d229bf5204c8fc6cab7e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5042145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966bdbd5f41b922365e541cf6121d6cf76a4ddb1f9c111e010656f7041d50c1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:c0f257aca3b8b7405bb5549a368de7ae62c806fe4e75e189b405a7ce1f65fa4b in /nats-server 
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:39:55 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:39:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:39:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12032ad6ebd443b7c142112d1df3d64b3deb3a403e0a99764593e5fe7843781b`  
		Last Modified: Mon, 09 Oct 2023 23:40:46 GMT  
		Size: 5.0 MB (5041638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7d34c174da06f5ab9c869a0197e492849a0d80fbf8f038f93e9e1ac634d1f7`  
		Last Modified: Mon, 09 Oct 2023 23:40:45 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore`

```console
$ docker pull nats@sha256:8dbf04badbb41fc71c6e2880ff3bbbfd4b117d6abced349307322c18e014c117
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2-windowsservercore` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:059aab4410ed4545cb5ce2d8dd236f0b5c3568341a60c48bd5a1cce6a34ad97f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037905706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d15e9ed22631845e0f6ab08ef7c67bfb34f20ef808833c7243bd894a1978af84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:32:18 GMT
ENV NATS_SERVER=2.10.2
# Wed, 11 Oct 2023 03:32:19 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.2/nats-server-v2.10.2-windows-amd64.zip
# Wed, 11 Oct 2023 03:32:21 GMT
ENV NATS_SERVER_SHASUM=ce8eed07736cc6e008b0d26808ec0cae5871a419d8e38b020cfd121d0f88b935
# Wed, 11 Oct 2023 03:34:22 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Oct 2023 03:36:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 11 Oct 2023 03:36:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:12 GMT
EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362b60e14057a139612c4649868ad03cdc62c387c1b84d4908aa5908f87e20ff`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64517fb064d3b69109b8e9f259256e0ef3f0adc49276790fb0e5fb4ece78cfc`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2263f3dafd6f25001f85eb3b171366a90f088823c95e5a559b5aa62ee251809`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bc429c4e89ff3ab7798f0ae3347e48b4979ea71a3740c2c0056936bc378ec0`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 438.0 KB (437960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f9316683d04ebbebf399d13c5de2e8c262b352dd1f08c6fbb0cf7911187aeb`  
		Last Modified: Wed, 11 Oct 2023 03:40:32 GMT  
		Size: 5.9 MB (5863943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd7967ce50710cf0aefd72c029cd070a7c29865152d227e1def2edb5d0f4365`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123be7b303544a1edb1cf1a28202059f984c7050377fe77230633e9f80a9658c`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218eeb362e2a56ad3bc9c71e196900056c5c067cc3cef638e395caa8dd31ff20`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f857db4d13bfffe59dac02cd3f605fb4ecaca8297626b1dbe54c6e27c82bb5`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:8dbf04badbb41fc71c6e2880ff3bbbfd4b117d6abced349307322c18e014c117
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:059aab4410ed4545cb5ce2d8dd236f0b5c3568341a60c48bd5a1cce6a34ad97f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037905706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d15e9ed22631845e0f6ab08ef7c67bfb34f20ef808833c7243bd894a1978af84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:32:18 GMT
ENV NATS_SERVER=2.10.2
# Wed, 11 Oct 2023 03:32:19 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.2/nats-server-v2.10.2-windows-amd64.zip
# Wed, 11 Oct 2023 03:32:21 GMT
ENV NATS_SERVER_SHASUM=ce8eed07736cc6e008b0d26808ec0cae5871a419d8e38b020cfd121d0f88b935
# Wed, 11 Oct 2023 03:34:22 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Oct 2023 03:36:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 11 Oct 2023 03:36:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:12 GMT
EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362b60e14057a139612c4649868ad03cdc62c387c1b84d4908aa5908f87e20ff`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64517fb064d3b69109b8e9f259256e0ef3f0adc49276790fb0e5fb4ece78cfc`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2263f3dafd6f25001f85eb3b171366a90f088823c95e5a559b5aa62ee251809`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bc429c4e89ff3ab7798f0ae3347e48b4979ea71a3740c2c0056936bc378ec0`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 438.0 KB (437960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f9316683d04ebbebf399d13c5de2e8c262b352dd1f08c6fbb0cf7911187aeb`  
		Last Modified: Wed, 11 Oct 2023 03:40:32 GMT  
		Size: 5.9 MB (5863943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd7967ce50710cf0aefd72c029cd070a7c29865152d227e1def2edb5d0f4365`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123be7b303544a1edb1cf1a28202059f984c7050377fe77230633e9f80a9658c`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218eeb362e2a56ad3bc9c71e196900056c5c067cc3cef638e395caa8dd31ff20`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f857db4d13bfffe59dac02cd3f605fb4ecaca8297626b1dbe54c6e27c82bb5`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10`

```console
$ docker pull nats@sha256:d1ad16d0eab77dc156d2434dc302bd575ad878757e1fe4603a560ca38d9fec26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4974; amd64

### `nats:2.10` - linux; amd64

```console
$ docker pull nats@sha256:7be2e854c9542ad2146d9baadede0f2e3d520d9ffc8b9ef24078852362d95c5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5469432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d633df072e1a202141ac94a984750c13337fede7f772b34400dc99a9285cd99`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:a7de81fdc98e0908f1fbfd4b16f2eeac146932aac03b4a109a89f93b3efbfc58 in /nats-server 
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:20:31 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:20:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:20:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:494ad87960e9c491e7d14b1b9a5ca82020e4b968c60a0f3bffece88c8cee4831`  
		Last Modified: Sun, 08 Oct 2023 12:45:05 GMT  
		Size: 5.5 MB (5468923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d4a6b4c3024603d5932b75b727d2b94f22a490f5326099a6112bf261dfebc5`  
		Last Modified: Mon, 09 Oct 2023 23:21:26 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10` - linux; arm variant v6

```console
$ docker pull nats@sha256:4311525539cb532e2215a0f0e6a97e456bf100aecae9df633068dce84725d3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5189188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b74620a2c8b938dece7aba41cf3db596039ac4579268f2083d879dc0338e3d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:78bf14fdba87d3f994b59ec64fa5f813ff988f0f91e4929c7aaf33d206d6e4e2 in /nats-server 
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:49:30 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:49:30 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:49:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:541bfb4a7866a6fb7234b9fb133b37cc8a1fff7bcf10779570793f66bfa36cc5`  
		Last Modified: Mon, 09 Oct 2023 23:50:25 GMT  
		Size: 5.2 MB (5188681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e9969a228338f491f74c367e86a77a512ae318604d924fa624ef4e9b944a62`  
		Last Modified: Mon, 09 Oct 2023 23:50:24 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10` - linux; arm variant v7

```console
$ docker pull nats@sha256:72a048e9abb13148a5588dd1f556af5cf11e91369fd856d21e1b981e2f0f6aec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3f7200638809e9d2ec5971ab53b5a84b4413d7fce360c58f1d7381d739555e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:dfba40eb121bd5821909fe10c59b498aec418c7224d18a7961e71444dc375765 in /nats-server 
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:57:51 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c24b02c85cdfcd5bdce9a848ef068ff9e9535a6287fb7a00eb8e39b357c54ad0`  
		Last Modified: Mon, 09 Oct 2023 23:58:40 GMT  
		Size: 5.2 MB (5177978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d844de696d0e40f4aff106f51467e397619526062047fe60f4b692adda3bd736`  
		Last Modified: Mon, 09 Oct 2023 23:58:39 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:4b167dea0c683971c7d06db669fbdebf2a8b3c01cb4d229bf5204c8fc6cab7e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5042145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966bdbd5f41b922365e541cf6121d6cf76a4ddb1f9c111e010656f7041d50c1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:c0f257aca3b8b7405bb5549a368de7ae62c806fe4e75e189b405a7ce1f65fa4b in /nats-server 
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:39:55 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:39:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:39:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12032ad6ebd443b7c142112d1df3d64b3deb3a403e0a99764593e5fe7843781b`  
		Last Modified: Mon, 09 Oct 2023 23:40:46 GMT  
		Size: 5.0 MB (5041638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7d34c174da06f5ab9c869a0197e492849a0d80fbf8f038f93e9e1ac634d1f7`  
		Last Modified: Mon, 09 Oct 2023 23:40:45 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:d0a9a23bc5e727b8b8db67f5a02c6be5d0dfba5700152d11e56457862713e866
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110053852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f669b1f92bc1e89b2470de199627f90a4496308a2cd8c5f8bfd06b52ecf39a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:36:34 GMT
RUN cmd /S /C #(nop) COPY file:56de93ec6afaefd5f19b9effd4409842fdfa695280fb05da230b1d12a03db7bb in C:\nats-server.exe 
# Wed, 11 Oct 2023 03:36:35 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52fe086e7510cd640f31a862cc7ed0aae171d6591241c4eddfbeda3169a718b`  
		Last Modified: Wed, 11 Oct 2023 03:40:51 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f15b99379f9a65c4a40e86d7f09407cf716ae5cdd5ec3fdfbcd609fceb69f5`  
		Last Modified: Wed, 11 Oct 2023 03:40:50 GMT  
		Size: 5.6 MB (5582847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3574203dd8b3d01c5d1979302e56d73e3c604318c215efb12f98e667c80879`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937e84807bea241751a5e003bbf2cca02d1a37306e3cd7d17e260322cebb9e70`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fde0249533da9dfa2f6b077b43c2290316223ac025f271a8ba383f1136ff00`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee3b7476b8b4cb6aa82268271e5e2971d380d8da227366182b80abcfacc961`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-alpine`

```console
$ docker pull nats@sha256:c6d778a0df2aeeec2399f1e1ce558d7b65e70adc7ef5ca13f2cf06b1f7654a08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10-alpine` - linux; amd64

```console
$ docker pull nats@sha256:d6a47f89f52342be07d213d493e0b71a80fc94ccc19edc9c8b17169e8d887fbe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9494811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18e20b07c9925b57a0846b64bffdab236ff0d02728bea2661094cb2f1088d89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:20:15 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:20:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:20:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:20:17 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:20:17 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:20:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:20:17 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793ee3203ddeae4265feedfeeb0176c5d046487786e6430ec414b466b7342687`  
		Last Modified: Mon, 09 Oct 2023 23:21:01 GMT  
		Size: 6.1 MB (6091846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0dd902fefeb39726cbb9025e935fabe591af4d39f448ddad514c70eb56a6002`  
		Last Modified: Mon, 09 Oct 2023 23:21:00 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7a1bcf5bcb5ad0317a82f43795966d7b0cf297054e112bc548fe8d0c881df9`  
		Last Modified: Mon, 09 Oct 2023 23:21:00 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:6d9d5fd5f91a7c3e45e2cac23df6f50393e2024ea69495d9233df8ba9503bdc8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8958058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11708ece1d9ad1b7baf64c1f3c5e3b7a38ef5d66e87c24ba859eb6272bc2694f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:49:18 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:49:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:49:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:49:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:49:21 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dece2e91316626c2aeb73fab796c9095ba11a38f43e17e03f3cea33bada9941e`  
		Last Modified: Mon, 09 Oct 2023 23:49:58 GMT  
		Size: 5.8 MB (5811761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0164ce1b0fe0ce335f0348dbf1ef83dca670a9bb6c3036586e38f45c257ab3`  
		Last Modified: Mon, 09 Oct 2023 23:49:57 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a6185289b767b3266aeff451a57e88263f01cbb1544b137dd118ad2aa87d88`  
		Last Modified: Mon, 09 Oct 2023 23:49:57 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:56973c518df167ff13997d599dd6f0f488eb2a00380d161395d001cbd82ef4f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8701812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c71794277a3ea4fd3358f79bd24730e7bff545f116dbae54391ff86f7b5ba91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:57:29 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:57:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:57:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:57:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:57:31 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:57:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1577c013973725bb512b6e87006f323da7dece18dc8d5cddf516ac8ac1bd3690`  
		Last Modified: Mon, 09 Oct 2023 23:58:15 GMT  
		Size: 5.8 MB (5800912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2989475d4fcb37e49592f48904864c46ac84f25ca502bbddacc54bddf27ec9a3`  
		Last Modified: Mon, 09 Oct 2023 23:58:14 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dca18857ae02bbc23b7a6d389a1036fd7822d30861d1f065a1fce1b2662745e`  
		Last Modified: Mon, 09 Oct 2023 23:58:14 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a1cc118cb20105a3d28409f6f0134779e37d691cdfc8340e26aa21bf5c1fcecb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8999244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c690558bd2217d60e3ef1f45a02405b0c52118f1c91dda8b42c091696af68306`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:39:44 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:39:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:39:47 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:39:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e016e40994857a38606186dc8f2061ac54ed621273f59128aa5c6d060fb22`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 5.7 MB (5666417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15cff88ae624a30801728dd1b20bb84f6e871846c236cf2613ec7c7fb6008f1`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68049c030ad10066e6a3a63f9d02398f98a4b8bf2104c8d22adb9aed0ff83e1`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-alpine3.18`

```console
$ docker pull nats@sha256:c6d778a0df2aeeec2399f1e1ce558d7b65e70adc7ef5ca13f2cf06b1f7654a08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:d6a47f89f52342be07d213d493e0b71a80fc94ccc19edc9c8b17169e8d887fbe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9494811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18e20b07c9925b57a0846b64bffdab236ff0d02728bea2661094cb2f1088d89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:20:15 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:20:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:20:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:20:17 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:20:17 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:20:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:20:17 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793ee3203ddeae4265feedfeeb0176c5d046487786e6430ec414b466b7342687`  
		Last Modified: Mon, 09 Oct 2023 23:21:01 GMT  
		Size: 6.1 MB (6091846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0dd902fefeb39726cbb9025e935fabe591af4d39f448ddad514c70eb56a6002`  
		Last Modified: Mon, 09 Oct 2023 23:21:00 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7a1bcf5bcb5ad0317a82f43795966d7b0cf297054e112bc548fe8d0c881df9`  
		Last Modified: Mon, 09 Oct 2023 23:21:00 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:6d9d5fd5f91a7c3e45e2cac23df6f50393e2024ea69495d9233df8ba9503bdc8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8958058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11708ece1d9ad1b7baf64c1f3c5e3b7a38ef5d66e87c24ba859eb6272bc2694f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:49:18 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:49:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:49:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:49:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:49:21 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dece2e91316626c2aeb73fab796c9095ba11a38f43e17e03f3cea33bada9941e`  
		Last Modified: Mon, 09 Oct 2023 23:49:58 GMT  
		Size: 5.8 MB (5811761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0164ce1b0fe0ce335f0348dbf1ef83dca670a9bb6c3036586e38f45c257ab3`  
		Last Modified: Mon, 09 Oct 2023 23:49:57 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a6185289b767b3266aeff451a57e88263f01cbb1544b137dd118ad2aa87d88`  
		Last Modified: Mon, 09 Oct 2023 23:49:57 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:56973c518df167ff13997d599dd6f0f488eb2a00380d161395d001cbd82ef4f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8701812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c71794277a3ea4fd3358f79bd24730e7bff545f116dbae54391ff86f7b5ba91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:57:29 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:57:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:57:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:57:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:57:31 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:57:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1577c013973725bb512b6e87006f323da7dece18dc8d5cddf516ac8ac1bd3690`  
		Last Modified: Mon, 09 Oct 2023 23:58:15 GMT  
		Size: 5.8 MB (5800912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2989475d4fcb37e49592f48904864c46ac84f25ca502bbddacc54bddf27ec9a3`  
		Last Modified: Mon, 09 Oct 2023 23:58:14 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dca18857ae02bbc23b7a6d389a1036fd7822d30861d1f065a1fce1b2662745e`  
		Last Modified: Mon, 09 Oct 2023 23:58:14 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a1cc118cb20105a3d28409f6f0134779e37d691cdfc8340e26aa21bf5c1fcecb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8999244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c690558bd2217d60e3ef1f45a02405b0c52118f1c91dda8b42c091696af68306`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:39:44 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:39:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:39:47 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:39:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e016e40994857a38606186dc8f2061ac54ed621273f59128aa5c6d060fb22`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 5.7 MB (5666417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15cff88ae624a30801728dd1b20bb84f6e871846c236cf2613ec7c7fb6008f1`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68049c030ad10066e6a3a63f9d02398f98a4b8bf2104c8d22adb9aed0ff83e1`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-linux`

```console
$ docker pull nats@sha256:6a7739943a7360813f70dba186b72c6aba2163f2809fce7672cc3657b62043ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10-linux` - linux; amd64

```console
$ docker pull nats@sha256:7be2e854c9542ad2146d9baadede0f2e3d520d9ffc8b9ef24078852362d95c5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5469432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d633df072e1a202141ac94a984750c13337fede7f772b34400dc99a9285cd99`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:a7de81fdc98e0908f1fbfd4b16f2eeac146932aac03b4a109a89f93b3efbfc58 in /nats-server 
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:20:31 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:20:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:20:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:494ad87960e9c491e7d14b1b9a5ca82020e4b968c60a0f3bffece88c8cee4831`  
		Last Modified: Sun, 08 Oct 2023 12:45:05 GMT  
		Size: 5.5 MB (5468923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d4a6b4c3024603d5932b75b727d2b94f22a490f5326099a6112bf261dfebc5`  
		Last Modified: Mon, 09 Oct 2023 23:21:26 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:4311525539cb532e2215a0f0e6a97e456bf100aecae9df633068dce84725d3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5189188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b74620a2c8b938dece7aba41cf3db596039ac4579268f2083d879dc0338e3d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:78bf14fdba87d3f994b59ec64fa5f813ff988f0f91e4929c7aaf33d206d6e4e2 in /nats-server 
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:49:30 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:49:30 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:49:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:541bfb4a7866a6fb7234b9fb133b37cc8a1fff7bcf10779570793f66bfa36cc5`  
		Last Modified: Mon, 09 Oct 2023 23:50:25 GMT  
		Size: 5.2 MB (5188681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e9969a228338f491f74c367e86a77a512ae318604d924fa624ef4e9b944a62`  
		Last Modified: Mon, 09 Oct 2023 23:50:24 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:72a048e9abb13148a5588dd1f556af5cf11e91369fd856d21e1b981e2f0f6aec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3f7200638809e9d2ec5971ab53b5a84b4413d7fce360c58f1d7381d739555e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:dfba40eb121bd5821909fe10c59b498aec418c7224d18a7961e71444dc375765 in /nats-server 
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:57:51 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c24b02c85cdfcd5bdce9a848ef068ff9e9535a6287fb7a00eb8e39b357c54ad0`  
		Last Modified: Mon, 09 Oct 2023 23:58:40 GMT  
		Size: 5.2 MB (5177978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d844de696d0e40f4aff106f51467e397619526062047fe60f4b692adda3bd736`  
		Last Modified: Mon, 09 Oct 2023 23:58:39 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:4b167dea0c683971c7d06db669fbdebf2a8b3c01cb4d229bf5204c8fc6cab7e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5042145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966bdbd5f41b922365e541cf6121d6cf76a4ddb1f9c111e010656f7041d50c1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:c0f257aca3b8b7405bb5549a368de7ae62c806fe4e75e189b405a7ce1f65fa4b in /nats-server 
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:39:55 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:39:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:39:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12032ad6ebd443b7c142112d1df3d64b3deb3a403e0a99764593e5fe7843781b`  
		Last Modified: Mon, 09 Oct 2023 23:40:46 GMT  
		Size: 5.0 MB (5041638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7d34c174da06f5ab9c869a0197e492849a0d80fbf8f038f93e9e1ac634d1f7`  
		Last Modified: Mon, 09 Oct 2023 23:40:45 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-nanoserver`

```console
$ docker pull nats@sha256:d2017f7731ec6420f52e2633c4567934fc67c6b1466820f14cf57a737f77433c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.10-nanoserver` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:d0a9a23bc5e727b8b8db67f5a02c6be5d0dfba5700152d11e56457862713e866
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110053852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f669b1f92bc1e89b2470de199627f90a4496308a2cd8c5f8bfd06b52ecf39a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:36:34 GMT
RUN cmd /S /C #(nop) COPY file:56de93ec6afaefd5f19b9effd4409842fdfa695280fb05da230b1d12a03db7bb in C:\nats-server.exe 
# Wed, 11 Oct 2023 03:36:35 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52fe086e7510cd640f31a862cc7ed0aae171d6591241c4eddfbeda3169a718b`  
		Last Modified: Wed, 11 Oct 2023 03:40:51 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f15b99379f9a65c4a40e86d7f09407cf716ae5cdd5ec3fdfbcd609fceb69f5`  
		Last Modified: Wed, 11 Oct 2023 03:40:50 GMT  
		Size: 5.6 MB (5582847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3574203dd8b3d01c5d1979302e56d73e3c604318c215efb12f98e667c80879`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937e84807bea241751a5e003bbf2cca02d1a37306e3cd7d17e260322cebb9e70`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fde0249533da9dfa2f6b077b43c2290316223ac025f271a8ba383f1136ff00`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee3b7476b8b4cb6aa82268271e5e2971d380d8da227366182b80abcfacc961`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-nanoserver-1809`

```console
$ docker pull nats@sha256:d2017f7731ec6420f52e2633c4567934fc67c6b1466820f14cf57a737f77433c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.10-nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:d0a9a23bc5e727b8b8db67f5a02c6be5d0dfba5700152d11e56457862713e866
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110053852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f669b1f92bc1e89b2470de199627f90a4496308a2cd8c5f8bfd06b52ecf39a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:36:34 GMT
RUN cmd /S /C #(nop) COPY file:56de93ec6afaefd5f19b9effd4409842fdfa695280fb05da230b1d12a03db7bb in C:\nats-server.exe 
# Wed, 11 Oct 2023 03:36:35 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52fe086e7510cd640f31a862cc7ed0aae171d6591241c4eddfbeda3169a718b`  
		Last Modified: Wed, 11 Oct 2023 03:40:51 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f15b99379f9a65c4a40e86d7f09407cf716ae5cdd5ec3fdfbcd609fceb69f5`  
		Last Modified: Wed, 11 Oct 2023 03:40:50 GMT  
		Size: 5.6 MB (5582847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3574203dd8b3d01c5d1979302e56d73e3c604318c215efb12f98e667c80879`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937e84807bea241751a5e003bbf2cca02d1a37306e3cd7d17e260322cebb9e70`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fde0249533da9dfa2f6b077b43c2290316223ac025f271a8ba383f1136ff00`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee3b7476b8b4cb6aa82268271e5e2971d380d8da227366182b80abcfacc961`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-scratch`

```console
$ docker pull nats@sha256:6a7739943a7360813f70dba186b72c6aba2163f2809fce7672cc3657b62043ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10-scratch` - linux; amd64

```console
$ docker pull nats@sha256:7be2e854c9542ad2146d9baadede0f2e3d520d9ffc8b9ef24078852362d95c5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5469432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d633df072e1a202141ac94a984750c13337fede7f772b34400dc99a9285cd99`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:a7de81fdc98e0908f1fbfd4b16f2eeac146932aac03b4a109a89f93b3efbfc58 in /nats-server 
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:20:31 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:20:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:20:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:494ad87960e9c491e7d14b1b9a5ca82020e4b968c60a0f3bffece88c8cee4831`  
		Last Modified: Sun, 08 Oct 2023 12:45:05 GMT  
		Size: 5.5 MB (5468923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d4a6b4c3024603d5932b75b727d2b94f22a490f5326099a6112bf261dfebc5`  
		Last Modified: Mon, 09 Oct 2023 23:21:26 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:4311525539cb532e2215a0f0e6a97e456bf100aecae9df633068dce84725d3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5189188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b74620a2c8b938dece7aba41cf3db596039ac4579268f2083d879dc0338e3d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:78bf14fdba87d3f994b59ec64fa5f813ff988f0f91e4929c7aaf33d206d6e4e2 in /nats-server 
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:49:30 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:49:30 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:49:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:541bfb4a7866a6fb7234b9fb133b37cc8a1fff7bcf10779570793f66bfa36cc5`  
		Last Modified: Mon, 09 Oct 2023 23:50:25 GMT  
		Size: 5.2 MB (5188681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e9969a228338f491f74c367e86a77a512ae318604d924fa624ef4e9b944a62`  
		Last Modified: Mon, 09 Oct 2023 23:50:24 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:72a048e9abb13148a5588dd1f556af5cf11e91369fd856d21e1b981e2f0f6aec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3f7200638809e9d2ec5971ab53b5a84b4413d7fce360c58f1d7381d739555e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:dfba40eb121bd5821909fe10c59b498aec418c7224d18a7961e71444dc375765 in /nats-server 
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:57:51 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c24b02c85cdfcd5bdce9a848ef068ff9e9535a6287fb7a00eb8e39b357c54ad0`  
		Last Modified: Mon, 09 Oct 2023 23:58:40 GMT  
		Size: 5.2 MB (5177978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d844de696d0e40f4aff106f51467e397619526062047fe60f4b692adda3bd736`  
		Last Modified: Mon, 09 Oct 2023 23:58:39 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:4b167dea0c683971c7d06db669fbdebf2a8b3c01cb4d229bf5204c8fc6cab7e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5042145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966bdbd5f41b922365e541cf6121d6cf76a4ddb1f9c111e010656f7041d50c1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:c0f257aca3b8b7405bb5549a368de7ae62c806fe4e75e189b405a7ce1f65fa4b in /nats-server 
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:39:55 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:39:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:39:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12032ad6ebd443b7c142112d1df3d64b3deb3a403e0a99764593e5fe7843781b`  
		Last Modified: Mon, 09 Oct 2023 23:40:46 GMT  
		Size: 5.0 MB (5041638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7d34c174da06f5ab9c869a0197e492849a0d80fbf8f038f93e9e1ac634d1f7`  
		Last Modified: Mon, 09 Oct 2023 23:40:45 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-windowsservercore`

```console
$ docker pull nats@sha256:8dbf04badbb41fc71c6e2880ff3bbbfd4b117d6abced349307322c18e014c117
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.10-windowsservercore` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:059aab4410ed4545cb5ce2d8dd236f0b5c3568341a60c48bd5a1cce6a34ad97f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037905706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d15e9ed22631845e0f6ab08ef7c67bfb34f20ef808833c7243bd894a1978af84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:32:18 GMT
ENV NATS_SERVER=2.10.2
# Wed, 11 Oct 2023 03:32:19 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.2/nats-server-v2.10.2-windows-amd64.zip
# Wed, 11 Oct 2023 03:32:21 GMT
ENV NATS_SERVER_SHASUM=ce8eed07736cc6e008b0d26808ec0cae5871a419d8e38b020cfd121d0f88b935
# Wed, 11 Oct 2023 03:34:22 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Oct 2023 03:36:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 11 Oct 2023 03:36:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:12 GMT
EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362b60e14057a139612c4649868ad03cdc62c387c1b84d4908aa5908f87e20ff`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64517fb064d3b69109b8e9f259256e0ef3f0adc49276790fb0e5fb4ece78cfc`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2263f3dafd6f25001f85eb3b171366a90f088823c95e5a559b5aa62ee251809`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bc429c4e89ff3ab7798f0ae3347e48b4979ea71a3740c2c0056936bc378ec0`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 438.0 KB (437960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f9316683d04ebbebf399d13c5de2e8c262b352dd1f08c6fbb0cf7911187aeb`  
		Last Modified: Wed, 11 Oct 2023 03:40:32 GMT  
		Size: 5.9 MB (5863943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd7967ce50710cf0aefd72c029cd070a7c29865152d227e1def2edb5d0f4365`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123be7b303544a1edb1cf1a28202059f984c7050377fe77230633e9f80a9658c`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218eeb362e2a56ad3bc9c71e196900056c5c067cc3cef638e395caa8dd31ff20`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f857db4d13bfffe59dac02cd3f605fb4ecaca8297626b1dbe54c6e27c82bb5`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10-windowsservercore-1809`

```console
$ docker pull nats@sha256:8dbf04badbb41fc71c6e2880ff3bbbfd4b117d6abced349307322c18e014c117
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.10-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:059aab4410ed4545cb5ce2d8dd236f0b5c3568341a60c48bd5a1cce6a34ad97f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037905706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d15e9ed22631845e0f6ab08ef7c67bfb34f20ef808833c7243bd894a1978af84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:32:18 GMT
ENV NATS_SERVER=2.10.2
# Wed, 11 Oct 2023 03:32:19 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.2/nats-server-v2.10.2-windows-amd64.zip
# Wed, 11 Oct 2023 03:32:21 GMT
ENV NATS_SERVER_SHASUM=ce8eed07736cc6e008b0d26808ec0cae5871a419d8e38b020cfd121d0f88b935
# Wed, 11 Oct 2023 03:34:22 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Oct 2023 03:36:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 11 Oct 2023 03:36:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:12 GMT
EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362b60e14057a139612c4649868ad03cdc62c387c1b84d4908aa5908f87e20ff`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64517fb064d3b69109b8e9f259256e0ef3f0adc49276790fb0e5fb4ece78cfc`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2263f3dafd6f25001f85eb3b171366a90f088823c95e5a559b5aa62ee251809`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bc429c4e89ff3ab7798f0ae3347e48b4979ea71a3740c2c0056936bc378ec0`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 438.0 KB (437960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f9316683d04ebbebf399d13c5de2e8c262b352dd1f08c6fbb0cf7911187aeb`  
		Last Modified: Wed, 11 Oct 2023 03:40:32 GMT  
		Size: 5.9 MB (5863943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd7967ce50710cf0aefd72c029cd070a7c29865152d227e1def2edb5d0f4365`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123be7b303544a1edb1cf1a28202059f984c7050377fe77230633e9f80a9658c`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218eeb362e2a56ad3bc9c71e196900056c5c067cc3cef638e395caa8dd31ff20`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f857db4d13bfffe59dac02cd3f605fb4ecaca8297626b1dbe54c6e27c82bb5`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.2`

```console
$ docker pull nats@sha256:d1ad16d0eab77dc156d2434dc302bd575ad878757e1fe4603a560ca38d9fec26
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.4974; amd64

### `nats:2.10.2` - linux; amd64

```console
$ docker pull nats@sha256:7be2e854c9542ad2146d9baadede0f2e3d520d9ffc8b9ef24078852362d95c5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5469432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d633df072e1a202141ac94a984750c13337fede7f772b34400dc99a9285cd99`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:a7de81fdc98e0908f1fbfd4b16f2eeac146932aac03b4a109a89f93b3efbfc58 in /nats-server 
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:20:31 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:20:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:20:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:494ad87960e9c491e7d14b1b9a5ca82020e4b968c60a0f3bffece88c8cee4831`  
		Last Modified: Sun, 08 Oct 2023 12:45:05 GMT  
		Size: 5.5 MB (5468923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d4a6b4c3024603d5932b75b727d2b94f22a490f5326099a6112bf261dfebc5`  
		Last Modified: Mon, 09 Oct 2023 23:21:26 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.2` - linux; arm variant v6

```console
$ docker pull nats@sha256:4311525539cb532e2215a0f0e6a97e456bf100aecae9df633068dce84725d3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5189188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b74620a2c8b938dece7aba41cf3db596039ac4579268f2083d879dc0338e3d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:78bf14fdba87d3f994b59ec64fa5f813ff988f0f91e4929c7aaf33d206d6e4e2 in /nats-server 
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:49:30 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:49:30 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:49:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:541bfb4a7866a6fb7234b9fb133b37cc8a1fff7bcf10779570793f66bfa36cc5`  
		Last Modified: Mon, 09 Oct 2023 23:50:25 GMT  
		Size: 5.2 MB (5188681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e9969a228338f491f74c367e86a77a512ae318604d924fa624ef4e9b944a62`  
		Last Modified: Mon, 09 Oct 2023 23:50:24 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.2` - linux; arm variant v7

```console
$ docker pull nats@sha256:72a048e9abb13148a5588dd1f556af5cf11e91369fd856d21e1b981e2f0f6aec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3f7200638809e9d2ec5971ab53b5a84b4413d7fce360c58f1d7381d739555e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:dfba40eb121bd5821909fe10c59b498aec418c7224d18a7961e71444dc375765 in /nats-server 
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:57:51 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c24b02c85cdfcd5bdce9a848ef068ff9e9535a6287fb7a00eb8e39b357c54ad0`  
		Last Modified: Mon, 09 Oct 2023 23:58:40 GMT  
		Size: 5.2 MB (5177978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d844de696d0e40f4aff106f51467e397619526062047fe60f4b692adda3bd736`  
		Last Modified: Mon, 09 Oct 2023 23:58:39 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.2` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:4b167dea0c683971c7d06db669fbdebf2a8b3c01cb4d229bf5204c8fc6cab7e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5042145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966bdbd5f41b922365e541cf6121d6cf76a4ddb1f9c111e010656f7041d50c1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:c0f257aca3b8b7405bb5549a368de7ae62c806fe4e75e189b405a7ce1f65fa4b in /nats-server 
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:39:55 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:39:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:39:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12032ad6ebd443b7c142112d1df3d64b3deb3a403e0a99764593e5fe7843781b`  
		Last Modified: Mon, 09 Oct 2023 23:40:46 GMT  
		Size: 5.0 MB (5041638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7d34c174da06f5ab9c869a0197e492849a0d80fbf8f038f93e9e1ac634d1f7`  
		Last Modified: Mon, 09 Oct 2023 23:40:45 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.2` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:d0a9a23bc5e727b8b8db67f5a02c6be5d0dfba5700152d11e56457862713e866
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110053852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f669b1f92bc1e89b2470de199627f90a4496308a2cd8c5f8bfd06b52ecf39a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:36:34 GMT
RUN cmd /S /C #(nop) COPY file:56de93ec6afaefd5f19b9effd4409842fdfa695280fb05da230b1d12a03db7bb in C:\nats-server.exe 
# Wed, 11 Oct 2023 03:36:35 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52fe086e7510cd640f31a862cc7ed0aae171d6591241c4eddfbeda3169a718b`  
		Last Modified: Wed, 11 Oct 2023 03:40:51 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f15b99379f9a65c4a40e86d7f09407cf716ae5cdd5ec3fdfbcd609fceb69f5`  
		Last Modified: Wed, 11 Oct 2023 03:40:50 GMT  
		Size: 5.6 MB (5582847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3574203dd8b3d01c5d1979302e56d73e3c604318c215efb12f98e667c80879`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937e84807bea241751a5e003bbf2cca02d1a37306e3cd7d17e260322cebb9e70`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fde0249533da9dfa2f6b077b43c2290316223ac025f271a8ba383f1136ff00`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee3b7476b8b4cb6aa82268271e5e2971d380d8da227366182b80abcfacc961`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.2-alpine`

```console
$ docker pull nats@sha256:c6d778a0df2aeeec2399f1e1ce558d7b65e70adc7ef5ca13f2cf06b1f7654a08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10.2-alpine` - linux; amd64

```console
$ docker pull nats@sha256:d6a47f89f52342be07d213d493e0b71a80fc94ccc19edc9c8b17169e8d887fbe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9494811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18e20b07c9925b57a0846b64bffdab236ff0d02728bea2661094cb2f1088d89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:20:15 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:20:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:20:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:20:17 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:20:17 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:20:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:20:17 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793ee3203ddeae4265feedfeeb0176c5d046487786e6430ec414b466b7342687`  
		Last Modified: Mon, 09 Oct 2023 23:21:01 GMT  
		Size: 6.1 MB (6091846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0dd902fefeb39726cbb9025e935fabe591af4d39f448ddad514c70eb56a6002`  
		Last Modified: Mon, 09 Oct 2023 23:21:00 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7a1bcf5bcb5ad0317a82f43795966d7b0cf297054e112bc548fe8d0c881df9`  
		Last Modified: Mon, 09 Oct 2023 23:21:00 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.2-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:6d9d5fd5f91a7c3e45e2cac23df6f50393e2024ea69495d9233df8ba9503bdc8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8958058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11708ece1d9ad1b7baf64c1f3c5e3b7a38ef5d66e87c24ba859eb6272bc2694f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:49:18 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:49:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:49:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:49:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:49:21 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dece2e91316626c2aeb73fab796c9095ba11a38f43e17e03f3cea33bada9941e`  
		Last Modified: Mon, 09 Oct 2023 23:49:58 GMT  
		Size: 5.8 MB (5811761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0164ce1b0fe0ce335f0348dbf1ef83dca670a9bb6c3036586e38f45c257ab3`  
		Last Modified: Mon, 09 Oct 2023 23:49:57 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a6185289b767b3266aeff451a57e88263f01cbb1544b137dd118ad2aa87d88`  
		Last Modified: Mon, 09 Oct 2023 23:49:57 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.2-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:56973c518df167ff13997d599dd6f0f488eb2a00380d161395d001cbd82ef4f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8701812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c71794277a3ea4fd3358f79bd24730e7bff545f116dbae54391ff86f7b5ba91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:57:29 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:57:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:57:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:57:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:57:31 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:57:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1577c013973725bb512b6e87006f323da7dece18dc8d5cddf516ac8ac1bd3690`  
		Last Modified: Mon, 09 Oct 2023 23:58:15 GMT  
		Size: 5.8 MB (5800912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2989475d4fcb37e49592f48904864c46ac84f25ca502bbddacc54bddf27ec9a3`  
		Last Modified: Mon, 09 Oct 2023 23:58:14 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dca18857ae02bbc23b7a6d389a1036fd7822d30861d1f065a1fce1b2662745e`  
		Last Modified: Mon, 09 Oct 2023 23:58:14 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.2-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a1cc118cb20105a3d28409f6f0134779e37d691cdfc8340e26aa21bf5c1fcecb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8999244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c690558bd2217d60e3ef1f45a02405b0c52118f1c91dda8b42c091696af68306`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:39:44 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:39:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:39:47 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:39:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e016e40994857a38606186dc8f2061ac54ed621273f59128aa5c6d060fb22`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 5.7 MB (5666417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15cff88ae624a30801728dd1b20bb84f6e871846c236cf2613ec7c7fb6008f1`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68049c030ad10066e6a3a63f9d02398f98a4b8bf2104c8d22adb9aed0ff83e1`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.2-alpine3.18`

```console
$ docker pull nats@sha256:c6d778a0df2aeeec2399f1e1ce558d7b65e70adc7ef5ca13f2cf06b1f7654a08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10.2-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:d6a47f89f52342be07d213d493e0b71a80fc94ccc19edc9c8b17169e8d887fbe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9494811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18e20b07c9925b57a0846b64bffdab236ff0d02728bea2661094cb2f1088d89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:20:15 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:20:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:20:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:20:17 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:20:17 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:20:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:20:17 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793ee3203ddeae4265feedfeeb0176c5d046487786e6430ec414b466b7342687`  
		Last Modified: Mon, 09 Oct 2023 23:21:01 GMT  
		Size: 6.1 MB (6091846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0dd902fefeb39726cbb9025e935fabe591af4d39f448ddad514c70eb56a6002`  
		Last Modified: Mon, 09 Oct 2023 23:21:00 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7a1bcf5bcb5ad0317a82f43795966d7b0cf297054e112bc548fe8d0c881df9`  
		Last Modified: Mon, 09 Oct 2023 23:21:00 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.2-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:6d9d5fd5f91a7c3e45e2cac23df6f50393e2024ea69495d9233df8ba9503bdc8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8958058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11708ece1d9ad1b7baf64c1f3c5e3b7a38ef5d66e87c24ba859eb6272bc2694f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:49:18 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:49:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:49:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:49:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:49:21 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dece2e91316626c2aeb73fab796c9095ba11a38f43e17e03f3cea33bada9941e`  
		Last Modified: Mon, 09 Oct 2023 23:49:58 GMT  
		Size: 5.8 MB (5811761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0164ce1b0fe0ce335f0348dbf1ef83dca670a9bb6c3036586e38f45c257ab3`  
		Last Modified: Mon, 09 Oct 2023 23:49:57 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a6185289b767b3266aeff451a57e88263f01cbb1544b137dd118ad2aa87d88`  
		Last Modified: Mon, 09 Oct 2023 23:49:57 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.2-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:56973c518df167ff13997d599dd6f0f488eb2a00380d161395d001cbd82ef4f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8701812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c71794277a3ea4fd3358f79bd24730e7bff545f116dbae54391ff86f7b5ba91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:57:29 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:57:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:57:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:57:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:57:31 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:57:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1577c013973725bb512b6e87006f323da7dece18dc8d5cddf516ac8ac1bd3690`  
		Last Modified: Mon, 09 Oct 2023 23:58:15 GMT  
		Size: 5.8 MB (5800912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2989475d4fcb37e49592f48904864c46ac84f25ca502bbddacc54bddf27ec9a3`  
		Last Modified: Mon, 09 Oct 2023 23:58:14 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dca18857ae02bbc23b7a6d389a1036fd7822d30861d1f065a1fce1b2662745e`  
		Last Modified: Mon, 09 Oct 2023 23:58:14 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.2-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a1cc118cb20105a3d28409f6f0134779e37d691cdfc8340e26aa21bf5c1fcecb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8999244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c690558bd2217d60e3ef1f45a02405b0c52118f1c91dda8b42c091696af68306`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:39:44 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:39:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:39:47 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:39:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e016e40994857a38606186dc8f2061ac54ed621273f59128aa5c6d060fb22`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 5.7 MB (5666417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15cff88ae624a30801728dd1b20bb84f6e871846c236cf2613ec7c7fb6008f1`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68049c030ad10066e6a3a63f9d02398f98a4b8bf2104c8d22adb9aed0ff83e1`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.2-linux`

```console
$ docker pull nats@sha256:6a7739943a7360813f70dba186b72c6aba2163f2809fce7672cc3657b62043ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10.2-linux` - linux; amd64

```console
$ docker pull nats@sha256:7be2e854c9542ad2146d9baadede0f2e3d520d9ffc8b9ef24078852362d95c5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5469432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d633df072e1a202141ac94a984750c13337fede7f772b34400dc99a9285cd99`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:a7de81fdc98e0908f1fbfd4b16f2eeac146932aac03b4a109a89f93b3efbfc58 in /nats-server 
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:20:31 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:20:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:20:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:494ad87960e9c491e7d14b1b9a5ca82020e4b968c60a0f3bffece88c8cee4831`  
		Last Modified: Sun, 08 Oct 2023 12:45:05 GMT  
		Size: 5.5 MB (5468923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d4a6b4c3024603d5932b75b727d2b94f22a490f5326099a6112bf261dfebc5`  
		Last Modified: Mon, 09 Oct 2023 23:21:26 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:4311525539cb532e2215a0f0e6a97e456bf100aecae9df633068dce84725d3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5189188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b74620a2c8b938dece7aba41cf3db596039ac4579268f2083d879dc0338e3d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:78bf14fdba87d3f994b59ec64fa5f813ff988f0f91e4929c7aaf33d206d6e4e2 in /nats-server 
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:49:30 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:49:30 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:49:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:541bfb4a7866a6fb7234b9fb133b37cc8a1fff7bcf10779570793f66bfa36cc5`  
		Last Modified: Mon, 09 Oct 2023 23:50:25 GMT  
		Size: 5.2 MB (5188681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e9969a228338f491f74c367e86a77a512ae318604d924fa624ef4e9b944a62`  
		Last Modified: Mon, 09 Oct 2023 23:50:24 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:72a048e9abb13148a5588dd1f556af5cf11e91369fd856d21e1b981e2f0f6aec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3f7200638809e9d2ec5971ab53b5a84b4413d7fce360c58f1d7381d739555e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:dfba40eb121bd5821909fe10c59b498aec418c7224d18a7961e71444dc375765 in /nats-server 
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:57:51 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c24b02c85cdfcd5bdce9a848ef068ff9e9535a6287fb7a00eb8e39b357c54ad0`  
		Last Modified: Mon, 09 Oct 2023 23:58:40 GMT  
		Size: 5.2 MB (5177978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d844de696d0e40f4aff106f51467e397619526062047fe60f4b692adda3bd736`  
		Last Modified: Mon, 09 Oct 2023 23:58:39 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:4b167dea0c683971c7d06db669fbdebf2a8b3c01cb4d229bf5204c8fc6cab7e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5042145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966bdbd5f41b922365e541cf6121d6cf76a4ddb1f9c111e010656f7041d50c1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:c0f257aca3b8b7405bb5549a368de7ae62c806fe4e75e189b405a7ce1f65fa4b in /nats-server 
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:39:55 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:39:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:39:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12032ad6ebd443b7c142112d1df3d64b3deb3a403e0a99764593e5fe7843781b`  
		Last Modified: Mon, 09 Oct 2023 23:40:46 GMT  
		Size: 5.0 MB (5041638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7d34c174da06f5ab9c869a0197e492849a0d80fbf8f038f93e9e1ac634d1f7`  
		Last Modified: Mon, 09 Oct 2023 23:40:45 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.2-nanoserver`

```console
$ docker pull nats@sha256:d2017f7731ec6420f52e2633c4567934fc67c6b1466820f14cf57a737f77433c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.10.2-nanoserver` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:d0a9a23bc5e727b8b8db67f5a02c6be5d0dfba5700152d11e56457862713e866
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110053852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f669b1f92bc1e89b2470de199627f90a4496308a2cd8c5f8bfd06b52ecf39a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:36:34 GMT
RUN cmd /S /C #(nop) COPY file:56de93ec6afaefd5f19b9effd4409842fdfa695280fb05da230b1d12a03db7bb in C:\nats-server.exe 
# Wed, 11 Oct 2023 03:36:35 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52fe086e7510cd640f31a862cc7ed0aae171d6591241c4eddfbeda3169a718b`  
		Last Modified: Wed, 11 Oct 2023 03:40:51 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f15b99379f9a65c4a40e86d7f09407cf716ae5cdd5ec3fdfbcd609fceb69f5`  
		Last Modified: Wed, 11 Oct 2023 03:40:50 GMT  
		Size: 5.6 MB (5582847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3574203dd8b3d01c5d1979302e56d73e3c604318c215efb12f98e667c80879`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937e84807bea241751a5e003bbf2cca02d1a37306e3cd7d17e260322cebb9e70`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fde0249533da9dfa2f6b077b43c2290316223ac025f271a8ba383f1136ff00`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee3b7476b8b4cb6aa82268271e5e2971d380d8da227366182b80abcfacc961`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.2-nanoserver-1809`

```console
$ docker pull nats@sha256:d2017f7731ec6420f52e2633c4567934fc67c6b1466820f14cf57a737f77433c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.10.2-nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:d0a9a23bc5e727b8b8db67f5a02c6be5d0dfba5700152d11e56457862713e866
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110053852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f669b1f92bc1e89b2470de199627f90a4496308a2cd8c5f8bfd06b52ecf39a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:36:34 GMT
RUN cmd /S /C #(nop) COPY file:56de93ec6afaefd5f19b9effd4409842fdfa695280fb05da230b1d12a03db7bb in C:\nats-server.exe 
# Wed, 11 Oct 2023 03:36:35 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52fe086e7510cd640f31a862cc7ed0aae171d6591241c4eddfbeda3169a718b`  
		Last Modified: Wed, 11 Oct 2023 03:40:51 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f15b99379f9a65c4a40e86d7f09407cf716ae5cdd5ec3fdfbcd609fceb69f5`  
		Last Modified: Wed, 11 Oct 2023 03:40:50 GMT  
		Size: 5.6 MB (5582847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3574203dd8b3d01c5d1979302e56d73e3c604318c215efb12f98e667c80879`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937e84807bea241751a5e003bbf2cca02d1a37306e3cd7d17e260322cebb9e70`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fde0249533da9dfa2f6b077b43c2290316223ac025f271a8ba383f1136ff00`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee3b7476b8b4cb6aa82268271e5e2971d380d8da227366182b80abcfacc961`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.2-scratch`

```console
$ docker pull nats@sha256:6a7739943a7360813f70dba186b72c6aba2163f2809fce7672cc3657b62043ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.10.2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:7be2e854c9542ad2146d9baadede0f2e3d520d9ffc8b9ef24078852362d95c5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5469432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d633df072e1a202141ac94a984750c13337fede7f772b34400dc99a9285cd99`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:a7de81fdc98e0908f1fbfd4b16f2eeac146932aac03b4a109a89f93b3efbfc58 in /nats-server 
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:20:31 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:20:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:20:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:494ad87960e9c491e7d14b1b9a5ca82020e4b968c60a0f3bffece88c8cee4831`  
		Last Modified: Sun, 08 Oct 2023 12:45:05 GMT  
		Size: 5.5 MB (5468923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d4a6b4c3024603d5932b75b727d2b94f22a490f5326099a6112bf261dfebc5`  
		Last Modified: Mon, 09 Oct 2023 23:21:26 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:4311525539cb532e2215a0f0e6a97e456bf100aecae9df633068dce84725d3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5189188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b74620a2c8b938dece7aba41cf3db596039ac4579268f2083d879dc0338e3d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:78bf14fdba87d3f994b59ec64fa5f813ff988f0f91e4929c7aaf33d206d6e4e2 in /nats-server 
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:49:30 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:49:30 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:49:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:541bfb4a7866a6fb7234b9fb133b37cc8a1fff7bcf10779570793f66bfa36cc5`  
		Last Modified: Mon, 09 Oct 2023 23:50:25 GMT  
		Size: 5.2 MB (5188681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e9969a228338f491f74c367e86a77a512ae318604d924fa624ef4e9b944a62`  
		Last Modified: Mon, 09 Oct 2023 23:50:24 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.2-scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:72a048e9abb13148a5588dd1f556af5cf11e91369fd856d21e1b981e2f0f6aec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3f7200638809e9d2ec5971ab53b5a84b4413d7fce360c58f1d7381d739555e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:dfba40eb121bd5821909fe10c59b498aec418c7224d18a7961e71444dc375765 in /nats-server 
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:57:51 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c24b02c85cdfcd5bdce9a848ef068ff9e9535a6287fb7a00eb8e39b357c54ad0`  
		Last Modified: Mon, 09 Oct 2023 23:58:40 GMT  
		Size: 5.2 MB (5177978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d844de696d0e40f4aff106f51467e397619526062047fe60f4b692adda3bd736`  
		Last Modified: Mon, 09 Oct 2023 23:58:39 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.10.2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:4b167dea0c683971c7d06db669fbdebf2a8b3c01cb4d229bf5204c8fc6cab7e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5042145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966bdbd5f41b922365e541cf6121d6cf76a4ddb1f9c111e010656f7041d50c1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:c0f257aca3b8b7405bb5549a368de7ae62c806fe4e75e189b405a7ce1f65fa4b in /nats-server 
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:39:55 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:39:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:39:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12032ad6ebd443b7c142112d1df3d64b3deb3a403e0a99764593e5fe7843781b`  
		Last Modified: Mon, 09 Oct 2023 23:40:46 GMT  
		Size: 5.0 MB (5041638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7d34c174da06f5ab9c869a0197e492849a0d80fbf8f038f93e9e1ac634d1f7`  
		Last Modified: Mon, 09 Oct 2023 23:40:45 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.2-windowsservercore`

```console
$ docker pull nats@sha256:8dbf04badbb41fc71c6e2880ff3bbbfd4b117d6abced349307322c18e014c117
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.10.2-windowsservercore` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:059aab4410ed4545cb5ce2d8dd236f0b5c3568341a60c48bd5a1cce6a34ad97f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037905706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d15e9ed22631845e0f6ab08ef7c67bfb34f20ef808833c7243bd894a1978af84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:32:18 GMT
ENV NATS_SERVER=2.10.2
# Wed, 11 Oct 2023 03:32:19 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.2/nats-server-v2.10.2-windows-amd64.zip
# Wed, 11 Oct 2023 03:32:21 GMT
ENV NATS_SERVER_SHASUM=ce8eed07736cc6e008b0d26808ec0cae5871a419d8e38b020cfd121d0f88b935
# Wed, 11 Oct 2023 03:34:22 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Oct 2023 03:36:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 11 Oct 2023 03:36:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:12 GMT
EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362b60e14057a139612c4649868ad03cdc62c387c1b84d4908aa5908f87e20ff`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64517fb064d3b69109b8e9f259256e0ef3f0adc49276790fb0e5fb4ece78cfc`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2263f3dafd6f25001f85eb3b171366a90f088823c95e5a559b5aa62ee251809`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bc429c4e89ff3ab7798f0ae3347e48b4979ea71a3740c2c0056936bc378ec0`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 438.0 KB (437960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f9316683d04ebbebf399d13c5de2e8c262b352dd1f08c6fbb0cf7911187aeb`  
		Last Modified: Wed, 11 Oct 2023 03:40:32 GMT  
		Size: 5.9 MB (5863943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd7967ce50710cf0aefd72c029cd070a7c29865152d227e1def2edb5d0f4365`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123be7b303544a1edb1cf1a28202059f984c7050377fe77230633e9f80a9658c`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218eeb362e2a56ad3bc9c71e196900056c5c067cc3cef638e395caa8dd31ff20`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f857db4d13bfffe59dac02cd3f605fb4ecaca8297626b1dbe54c6e27c82bb5`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.10.2-windowsservercore-1809`

```console
$ docker pull nats@sha256:8dbf04badbb41fc71c6e2880ff3bbbfd4b117d6abced349307322c18e014c117
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.10.2-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:059aab4410ed4545cb5ce2d8dd236f0b5c3568341a60c48bd5a1cce6a34ad97f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037905706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d15e9ed22631845e0f6ab08ef7c67bfb34f20ef808833c7243bd894a1978af84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:32:18 GMT
ENV NATS_SERVER=2.10.2
# Wed, 11 Oct 2023 03:32:19 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.2/nats-server-v2.10.2-windows-amd64.zip
# Wed, 11 Oct 2023 03:32:21 GMT
ENV NATS_SERVER_SHASUM=ce8eed07736cc6e008b0d26808ec0cae5871a419d8e38b020cfd121d0f88b935
# Wed, 11 Oct 2023 03:34:22 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Oct 2023 03:36:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 11 Oct 2023 03:36:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:12 GMT
EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362b60e14057a139612c4649868ad03cdc62c387c1b84d4908aa5908f87e20ff`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64517fb064d3b69109b8e9f259256e0ef3f0adc49276790fb0e5fb4ece78cfc`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2263f3dafd6f25001f85eb3b171366a90f088823c95e5a559b5aa62ee251809`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bc429c4e89ff3ab7798f0ae3347e48b4979ea71a3740c2c0056936bc378ec0`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 438.0 KB (437960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f9316683d04ebbebf399d13c5de2e8c262b352dd1f08c6fbb0cf7911187aeb`  
		Last Modified: Wed, 11 Oct 2023 03:40:32 GMT  
		Size: 5.9 MB (5863943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd7967ce50710cf0aefd72c029cd070a7c29865152d227e1def2edb5d0f4365`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123be7b303544a1edb1cf1a28202059f984c7050377fe77230633e9f80a9658c`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218eeb362e2a56ad3bc9c71e196900056c5c067cc3cef638e395caa8dd31ff20`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f857db4d13bfffe59dac02cd3f605fb4ecaca8297626b1dbe54c6e27c82bb5`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1430 bytes)  
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
$ docker pull nats@sha256:e56e30eb3763a62b66ae1970fb8e950879a347724f75e79fbc7d58f194dc8ef7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine` - linux; amd64

```console
$ docker pull nats@sha256:ea7a019f8f71ab49206a746200be09e7fab2b2319e21bdad84494942eea5129b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9270749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4444ddccb29b2fad602512a5c072a5b423f530cd9ca1b62dc2fd2fafb844628e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:03:56 GMT
ENV NATS_SERVER=2.9.22
# Thu, 28 Sep 2023 23:03:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 28 Sep 2023 23:03:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 28 Sep 2023 23:03:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Sep 2023 23:03:59 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Sep 2023 23:03:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 23:03:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344ddae942421f08eba2d35ca5fb15207c059b05611526f2634f4f783b313195`  
		Last Modified: Thu, 28 Sep 2023 23:04:59 GMT  
		Size: 5.9 MB (5867784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4ca948a616cb91c19cc7459b10b01c913677097d2bdc189c43d67a1a467011`  
		Last Modified: Thu, 28 Sep 2023 23:04:58 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429d044774dd68c36cd852a3a4486eb7da37c248e4ba4100bfa20c5ecfab4cba`  
		Last Modified: Thu, 28 Sep 2023 23:04:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:9b13e03d487b41ad6e6201b9203fea9e88fad106d46dfd8514914f98a6bb98fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8749587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c342f1da19613cc424e3d59b510a8036b9a5239296ae2b7340e284376a6be9a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:11:22 GMT
ENV NATS_SERVER=2.9.22
# Thu, 28 Sep 2023 22:11:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 28 Sep 2023 22:11:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 28 Sep 2023 22:11:25 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Sep 2023 22:11:25 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Sep 2023 22:11:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 22:11:26 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630c915de7bdf058602fd319c5ad749f49f9eb9bacd5dd06e9ca18175eb84cad`  
		Last Modified: Thu, 28 Sep 2023 22:12:18 GMT  
		Size: 5.6 MB (5603293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc58f097ef6a2be1e278bae3263fedc9e6f5bf946000f3d48d677a165f4f402`  
		Last Modified: Thu, 28 Sep 2023 22:12:17 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f5692ecd59317b7715ef39bf4c3e08335f62de978373f2e7b0f242b553b54f`  
		Last Modified: Thu, 28 Sep 2023 22:12:17 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:e6da5cc898bfdc25941dd437e96b9a961843df4116dcb0f3ed31412d37a98493
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8493289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee203567cc45c4a8288b4650f2afc365f43eb01c42fac9f92c3063cacd70c332`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:17:49 GMT
ENV NATS_SERVER=2.9.22
# Thu, 28 Sep 2023 23:17:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 28 Sep 2023 23:17:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 28 Sep 2023 23:17:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Sep 2023 23:17:51 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Sep 2023 23:17:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 23:17:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e6799cc112563f5bd57ccf66b5ae4e1acb9b0f9380f8ea5ff99bcdf394d87a`  
		Last Modified: Thu, 28 Sep 2023 23:18:48 GMT  
		Size: 5.6 MB (5592383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c2d8b97f2ee1947b9f1567d20195023a527212ead9b2fd1fc84c2c10f31282`  
		Last Modified: Thu, 28 Sep 2023 23:18:47 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b817a337dea1e3c1d94395fec370c3af29bd89dbb0149d57dd4b93c72cb9de`  
		Last Modified: Thu, 28 Sep 2023 23:18:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:974daab09263e17e09f36c429cdfa842c86e7f2a7f727e73ffa8d72a0c758228
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8735321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:010bd6c9016879b86bd554939bd0f2be66a0aeb82d807fe7288519980f99879d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:05:37 GMT
ENV NATS_SERVER=2.9.22
# Fri, 29 Sep 2023 02:05:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 29 Sep 2023 02:05:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 29 Sep 2023 02:05:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 29 Sep 2023 02:05:39 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Sep 2023 02:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 02:05:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76dd4ee8336fd067d1c11dd90428c4b26bc79b3521db6ba65309bfd68fcfe6b3`  
		Last Modified: Fri, 29 Sep 2023 02:06:41 GMT  
		Size: 5.4 MB (5402492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7966cb0b0f8d4873987436d855fcb89402026d7357cf9799ebd7636393c7e55e`  
		Last Modified: Fri, 29 Sep 2023 02:06:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6944ab51200e30863838a2feffd3da50d117f096e4dec219cedaa5b62dff1249`  
		Last Modified: Fri, 29 Sep 2023 02:06:40 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-alpine3.18`

```console
$ docker pull nats@sha256:e56e30eb3763a62b66ae1970fb8e950879a347724f75e79fbc7d58f194dc8ef7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:ea7a019f8f71ab49206a746200be09e7fab2b2319e21bdad84494942eea5129b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9270749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4444ddccb29b2fad602512a5c072a5b423f530cd9ca1b62dc2fd2fafb844628e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:03:56 GMT
ENV NATS_SERVER=2.9.22
# Thu, 28 Sep 2023 23:03:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 28 Sep 2023 23:03:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 28 Sep 2023 23:03:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Sep 2023 23:03:59 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Sep 2023 23:03:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 23:03:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344ddae942421f08eba2d35ca5fb15207c059b05611526f2634f4f783b313195`  
		Last Modified: Thu, 28 Sep 2023 23:04:59 GMT  
		Size: 5.9 MB (5867784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4ca948a616cb91c19cc7459b10b01c913677097d2bdc189c43d67a1a467011`  
		Last Modified: Thu, 28 Sep 2023 23:04:58 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429d044774dd68c36cd852a3a4486eb7da37c248e4ba4100bfa20c5ecfab4cba`  
		Last Modified: Thu, 28 Sep 2023 23:04:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:9b13e03d487b41ad6e6201b9203fea9e88fad106d46dfd8514914f98a6bb98fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8749587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c342f1da19613cc424e3d59b510a8036b9a5239296ae2b7340e284376a6be9a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:11:22 GMT
ENV NATS_SERVER=2.9.22
# Thu, 28 Sep 2023 22:11:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 28 Sep 2023 22:11:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 28 Sep 2023 22:11:25 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Sep 2023 22:11:25 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Sep 2023 22:11:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 22:11:26 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630c915de7bdf058602fd319c5ad749f49f9eb9bacd5dd06e9ca18175eb84cad`  
		Last Modified: Thu, 28 Sep 2023 22:12:18 GMT  
		Size: 5.6 MB (5603293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc58f097ef6a2be1e278bae3263fedc9e6f5bf946000f3d48d677a165f4f402`  
		Last Modified: Thu, 28 Sep 2023 22:12:17 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f5692ecd59317b7715ef39bf4c3e08335f62de978373f2e7b0f242b553b54f`  
		Last Modified: Thu, 28 Sep 2023 22:12:17 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:e6da5cc898bfdc25941dd437e96b9a961843df4116dcb0f3ed31412d37a98493
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8493289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee203567cc45c4a8288b4650f2afc365f43eb01c42fac9f92c3063cacd70c332`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:17:49 GMT
ENV NATS_SERVER=2.9.22
# Thu, 28 Sep 2023 23:17:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 28 Sep 2023 23:17:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 28 Sep 2023 23:17:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Sep 2023 23:17:51 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Sep 2023 23:17:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 23:17:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e6799cc112563f5bd57ccf66b5ae4e1acb9b0f9380f8ea5ff99bcdf394d87a`  
		Last Modified: Thu, 28 Sep 2023 23:18:48 GMT  
		Size: 5.6 MB (5592383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c2d8b97f2ee1947b9f1567d20195023a527212ead9b2fd1fc84c2c10f31282`  
		Last Modified: Thu, 28 Sep 2023 23:18:47 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b817a337dea1e3c1d94395fec370c3af29bd89dbb0149d57dd4b93c72cb9de`  
		Last Modified: Thu, 28 Sep 2023 23:18:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:974daab09263e17e09f36c429cdfa842c86e7f2a7f727e73ffa8d72a0c758228
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8735321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:010bd6c9016879b86bd554939bd0f2be66a0aeb82d807fe7288519980f99879d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:05:37 GMT
ENV NATS_SERVER=2.9.22
# Fri, 29 Sep 2023 02:05:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 29 Sep 2023 02:05:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 29 Sep 2023 02:05:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 29 Sep 2023 02:05:39 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Sep 2023 02:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 02:05:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76dd4ee8336fd067d1c11dd90428c4b26bc79b3521db6ba65309bfd68fcfe6b3`  
		Last Modified: Fri, 29 Sep 2023 02:06:41 GMT  
		Size: 5.4 MB (5402492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7966cb0b0f8d4873987436d855fcb89402026d7357cf9799ebd7636393c7e55e`  
		Last Modified: Fri, 29 Sep 2023 02:06:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6944ab51200e30863838a2feffd3da50d117f096e4dec219cedaa5b62dff1249`  
		Last Modified: Fri, 29 Sep 2023 02:06:40 GMT  
		Size: 412.0 B  
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
$ docker pull nats@sha256:f1b504cc4d7a24a79cb3ec47cc7968cfaa56398af6f0a56c9b8f02c11e87e198
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.9-nanoserver` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:f5b7c7052aa1d091ef81f5cb49a31d3629b21ae5da1d018cae367e601bec0a6d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109791051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea9c2e90f2e383203bae762574ce31298840db6117cf2b43de8f73e2d8ad3e33`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:39:57 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 11 Oct 2023 03:39:58 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:39:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:39:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:40:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52fe086e7510cd640f31a862cc7ed0aae171d6591241c4eddfbeda3169a718b`  
		Last Modified: Wed, 11 Oct 2023 03:40:51 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6759c77fac899cf8e1905cc3ae8d80c50b89decfa9054624b3dd6f460076e9`  
		Last Modified: Wed, 11 Oct 2023 03:41:16 GMT  
		Size: 5.3 MB (5320077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7158fb411ea29a9e1b6be836314c1ba4116d7ff26e4f4b8fa471d96f745bf64`  
		Last Modified: Wed, 11 Oct 2023 03:41:15 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f7a5bb7f58543897c1f653f0aaf27d5cb41a6bc23e9d58aa4977e7c6a56b0f`  
		Last Modified: Wed, 11 Oct 2023 03:41:15 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ea4b403539176bffc7b5217fa85130223e1b0593d5535c7ee5bca120a4e471`  
		Last Modified: Wed, 11 Oct 2023 03:41:15 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff475aa742bc198c00f6e55c4f40c431e460d7272bb78e4a187a8476d7a8ac36`  
		Last Modified: Wed, 11 Oct 2023 03:41:15 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-nanoserver-1809`

```console
$ docker pull nats@sha256:f1b504cc4d7a24a79cb3ec47cc7968cfaa56398af6f0a56c9b8f02c11e87e198
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.9-nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:f5b7c7052aa1d091ef81f5cb49a31d3629b21ae5da1d018cae367e601bec0a6d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109791051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea9c2e90f2e383203bae762574ce31298840db6117cf2b43de8f73e2d8ad3e33`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:39:57 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 11 Oct 2023 03:39:58 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:39:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:39:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:40:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52fe086e7510cd640f31a862cc7ed0aae171d6591241c4eddfbeda3169a718b`  
		Last Modified: Wed, 11 Oct 2023 03:40:51 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6759c77fac899cf8e1905cc3ae8d80c50b89decfa9054624b3dd6f460076e9`  
		Last Modified: Wed, 11 Oct 2023 03:41:16 GMT  
		Size: 5.3 MB (5320077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7158fb411ea29a9e1b6be836314c1ba4116d7ff26e4f4b8fa471d96f745bf64`  
		Last Modified: Wed, 11 Oct 2023 03:41:15 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f7a5bb7f58543897c1f653f0aaf27d5cb41a6bc23e9d58aa4977e7c6a56b0f`  
		Last Modified: Wed, 11 Oct 2023 03:41:15 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ea4b403539176bffc7b5217fa85130223e1b0593d5535c7ee5bca120a4e471`  
		Last Modified: Wed, 11 Oct 2023 03:41:15 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff475aa742bc198c00f6e55c4f40c431e460d7272bb78e4a187a8476d7a8ac36`  
		Last Modified: Wed, 11 Oct 2023 03:41:15 GMT  
		Size: 1.1 KB (1122 bytes)  
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
$ docker pull nats@sha256:a6425c9ec006beb738a167a459028fcca9f282e4e40d042284598a09b702a556
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.9-windowsservercore` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:045eb82cccf069cd433f0ea1844ca371c31bbb6a5100948a1c86b0847cc16775
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037669001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ece444de41a3389ace76622ea181809ffd86c614acbf5391eac86a523c8c1424`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:36:44 GMT
ENV NATS_SERVER=2.9.22
# Wed, 11 Oct 2023 03:36:45 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.22/nats-server-v2.9.22-windows-amd64.zip
# Wed, 11 Oct 2023 03:36:45 GMT
ENV NATS_SERVER_SHASUM=e91db73b02bd4dca3eb7a4bf32e29763450b08d593f73e87d0a6b70102dea0d4
# Wed, 11 Oct 2023 03:37:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Oct 2023 03:39:38 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 11 Oct 2023 03:39:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:39:40 GMT
EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:39:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:39:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d90788f0e55a4514b4130734c279ec44aca19b7b33db65a550c03f6c561ce4`  
		Last Modified: Wed, 11 Oct 2023 03:41:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa1528cb66af3af51f6a26e9a32fd00b8b7f1faa43e41bbe9f7b9077edd3ccf`  
		Last Modified: Wed, 11 Oct 2023 03:41:06 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9de9a1d29daf2f2518d42cbe7b08de42ee77f7b41f78e73437d193ea371bdd`  
		Last Modified: Wed, 11 Oct 2023 03:41:06 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea5bc356f3bfa68b3ca0a3129a9c4fd9d525eb71b58350c1ebd9780c851892`  
		Last Modified: Wed, 11 Oct 2023 03:41:06 GMT  
		Size: 450.5 KB (450507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb555481fabd89853d836bedfbe8efa7ee84b0e2cb440a37fb2a9ffbb96f7cfe`  
		Last Modified: Wed, 11 Oct 2023 03:41:05 GMT  
		Size: 5.6 MB (5614696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03163c07b0721c4a1d3270ccb7a7ace36fcee5c6550af64cb5c55b6d44ee772c`  
		Last Modified: Wed, 11 Oct 2023 03:41:04 GMT  
		Size: 2.0 KB (1966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fc000c6fcb389bf91057cc7a3f58c2dbf03e5bbe6aec78af7d96924c1176ae`  
		Last Modified: Wed, 11 Oct 2023 03:41:04 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5654a35313bcb88698d7d7db013197bd621a2cc8c3e6812ebc7000216ee451d9`  
		Last Modified: Wed, 11 Oct 2023 03:41:04 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caa0710f11b36a20354b2d9a9fd224b7c3fb6bc443f0350dfdf0655df236a92`  
		Last Modified: Wed, 11 Oct 2023 03:41:04 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9-windowsservercore-1809`

```console
$ docker pull nats@sha256:a6425c9ec006beb738a167a459028fcca9f282e4e40d042284598a09b702a556
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.9-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:045eb82cccf069cd433f0ea1844ca371c31bbb6a5100948a1c86b0847cc16775
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037669001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ece444de41a3389ace76622ea181809ffd86c614acbf5391eac86a523c8c1424`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:36:44 GMT
ENV NATS_SERVER=2.9.22
# Wed, 11 Oct 2023 03:36:45 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.22/nats-server-v2.9.22-windows-amd64.zip
# Wed, 11 Oct 2023 03:36:45 GMT
ENV NATS_SERVER_SHASUM=e91db73b02bd4dca3eb7a4bf32e29763450b08d593f73e87d0a6b70102dea0d4
# Wed, 11 Oct 2023 03:37:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Oct 2023 03:39:38 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 11 Oct 2023 03:39:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:39:40 GMT
EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:39:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:39:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d90788f0e55a4514b4130734c279ec44aca19b7b33db65a550c03f6c561ce4`  
		Last Modified: Wed, 11 Oct 2023 03:41:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa1528cb66af3af51f6a26e9a32fd00b8b7f1faa43e41bbe9f7b9077edd3ccf`  
		Last Modified: Wed, 11 Oct 2023 03:41:06 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9de9a1d29daf2f2518d42cbe7b08de42ee77f7b41f78e73437d193ea371bdd`  
		Last Modified: Wed, 11 Oct 2023 03:41:06 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea5bc356f3bfa68b3ca0a3129a9c4fd9d525eb71b58350c1ebd9780c851892`  
		Last Modified: Wed, 11 Oct 2023 03:41:06 GMT  
		Size: 450.5 KB (450507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb555481fabd89853d836bedfbe8efa7ee84b0e2cb440a37fb2a9ffbb96f7cfe`  
		Last Modified: Wed, 11 Oct 2023 03:41:05 GMT  
		Size: 5.6 MB (5614696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03163c07b0721c4a1d3270ccb7a7ace36fcee5c6550af64cb5c55b6d44ee772c`  
		Last Modified: Wed, 11 Oct 2023 03:41:04 GMT  
		Size: 2.0 KB (1966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fc000c6fcb389bf91057cc7a3f58c2dbf03e5bbe6aec78af7d96924c1176ae`  
		Last Modified: Wed, 11 Oct 2023 03:41:04 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5654a35313bcb88698d7d7db013197bd621a2cc8c3e6812ebc7000216ee451d9`  
		Last Modified: Wed, 11 Oct 2023 03:41:04 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caa0710f11b36a20354b2d9a9fd224b7c3fb6bc443f0350dfdf0655df236a92`  
		Last Modified: Wed, 11 Oct 2023 03:41:04 GMT  
		Size: 1.4 KB (1421 bytes)  
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
$ docker pull nats@sha256:e56e30eb3763a62b66ae1970fb8e950879a347724f75e79fbc7d58f194dc8ef7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.22-alpine` - linux; amd64

```console
$ docker pull nats@sha256:ea7a019f8f71ab49206a746200be09e7fab2b2319e21bdad84494942eea5129b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9270749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4444ddccb29b2fad602512a5c072a5b423f530cd9ca1b62dc2fd2fafb844628e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:03:56 GMT
ENV NATS_SERVER=2.9.22
# Thu, 28 Sep 2023 23:03:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 28 Sep 2023 23:03:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 28 Sep 2023 23:03:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Sep 2023 23:03:59 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Sep 2023 23:03:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 23:03:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344ddae942421f08eba2d35ca5fb15207c059b05611526f2634f4f783b313195`  
		Last Modified: Thu, 28 Sep 2023 23:04:59 GMT  
		Size: 5.9 MB (5867784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4ca948a616cb91c19cc7459b10b01c913677097d2bdc189c43d67a1a467011`  
		Last Modified: Thu, 28 Sep 2023 23:04:58 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429d044774dd68c36cd852a3a4486eb7da37c248e4ba4100bfa20c5ecfab4cba`  
		Last Modified: Thu, 28 Sep 2023 23:04:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:9b13e03d487b41ad6e6201b9203fea9e88fad106d46dfd8514914f98a6bb98fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8749587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c342f1da19613cc424e3d59b510a8036b9a5239296ae2b7340e284376a6be9a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:11:22 GMT
ENV NATS_SERVER=2.9.22
# Thu, 28 Sep 2023 22:11:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 28 Sep 2023 22:11:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 28 Sep 2023 22:11:25 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Sep 2023 22:11:25 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Sep 2023 22:11:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 22:11:26 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630c915de7bdf058602fd319c5ad749f49f9eb9bacd5dd06e9ca18175eb84cad`  
		Last Modified: Thu, 28 Sep 2023 22:12:18 GMT  
		Size: 5.6 MB (5603293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc58f097ef6a2be1e278bae3263fedc9e6f5bf946000f3d48d677a165f4f402`  
		Last Modified: Thu, 28 Sep 2023 22:12:17 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f5692ecd59317b7715ef39bf4c3e08335f62de978373f2e7b0f242b553b54f`  
		Last Modified: Thu, 28 Sep 2023 22:12:17 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:e6da5cc898bfdc25941dd437e96b9a961843df4116dcb0f3ed31412d37a98493
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8493289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee203567cc45c4a8288b4650f2afc365f43eb01c42fac9f92c3063cacd70c332`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:17:49 GMT
ENV NATS_SERVER=2.9.22
# Thu, 28 Sep 2023 23:17:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 28 Sep 2023 23:17:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 28 Sep 2023 23:17:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Sep 2023 23:17:51 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Sep 2023 23:17:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 23:17:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e6799cc112563f5bd57ccf66b5ae4e1acb9b0f9380f8ea5ff99bcdf394d87a`  
		Last Modified: Thu, 28 Sep 2023 23:18:48 GMT  
		Size: 5.6 MB (5592383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c2d8b97f2ee1947b9f1567d20195023a527212ead9b2fd1fc84c2c10f31282`  
		Last Modified: Thu, 28 Sep 2023 23:18:47 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b817a337dea1e3c1d94395fec370c3af29bd89dbb0149d57dd4b93c72cb9de`  
		Last Modified: Thu, 28 Sep 2023 23:18:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:974daab09263e17e09f36c429cdfa842c86e7f2a7f727e73ffa8d72a0c758228
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8735321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:010bd6c9016879b86bd554939bd0f2be66a0aeb82d807fe7288519980f99879d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:05:37 GMT
ENV NATS_SERVER=2.9.22
# Fri, 29 Sep 2023 02:05:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 29 Sep 2023 02:05:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 29 Sep 2023 02:05:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 29 Sep 2023 02:05:39 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Sep 2023 02:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 02:05:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76dd4ee8336fd067d1c11dd90428c4b26bc79b3521db6ba65309bfd68fcfe6b3`  
		Last Modified: Fri, 29 Sep 2023 02:06:41 GMT  
		Size: 5.4 MB (5402492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7966cb0b0f8d4873987436d855fcb89402026d7357cf9799ebd7636393c7e55e`  
		Last Modified: Fri, 29 Sep 2023 02:06:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6944ab51200e30863838a2feffd3da50d117f096e4dec219cedaa5b62dff1249`  
		Last Modified: Fri, 29 Sep 2023 02:06:40 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22-alpine3.18`

```console
$ docker pull nats@sha256:e56e30eb3763a62b66ae1970fb8e950879a347724f75e79fbc7d58f194dc8ef7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2.9.22-alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:ea7a019f8f71ab49206a746200be09e7fab2b2319e21bdad84494942eea5129b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.3 MB (9270749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4444ddccb29b2fad602512a5c072a5b423f530cd9ca1b62dc2fd2fafb844628e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:03:56 GMT
ENV NATS_SERVER=2.9.22
# Thu, 28 Sep 2023 23:03:58 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 28 Sep 2023 23:03:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 28 Sep 2023 23:03:58 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Sep 2023 23:03:59 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Sep 2023 23:03:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 23:03:59 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344ddae942421f08eba2d35ca5fb15207c059b05611526f2634f4f783b313195`  
		Last Modified: Thu, 28 Sep 2023 23:04:59 GMT  
		Size: 5.9 MB (5867784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b4ca948a616cb91c19cc7459b10b01c913677097d2bdc189c43d67a1a467011`  
		Last Modified: Thu, 28 Sep 2023 23:04:58 GMT  
		Size: 585.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429d044774dd68c36cd852a3a4486eb7da37c248e4ba4100bfa20c5ecfab4cba`  
		Last Modified: Thu, 28 Sep 2023 23:04:58 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:9b13e03d487b41ad6e6201b9203fea9e88fad106d46dfd8514914f98a6bb98fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8749587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c342f1da19613cc424e3d59b510a8036b9a5239296ae2b7340e284376a6be9a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 22:11:22 GMT
ENV NATS_SERVER=2.9.22
# Thu, 28 Sep 2023 22:11:25 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 28 Sep 2023 22:11:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 28 Sep 2023 22:11:25 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Sep 2023 22:11:25 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Sep 2023 22:11:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 22:11:26 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630c915de7bdf058602fd319c5ad749f49f9eb9bacd5dd06e9ca18175eb84cad`  
		Last Modified: Thu, 28 Sep 2023 22:12:18 GMT  
		Size: 5.6 MB (5603293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edc58f097ef6a2be1e278bae3263fedc9e6f5bf946000f3d48d677a165f4f402`  
		Last Modified: Thu, 28 Sep 2023 22:12:17 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f5692ecd59317b7715ef39bf4c3e08335f62de978373f2e7b0f242b553b54f`  
		Last Modified: Thu, 28 Sep 2023 22:12:17 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:e6da5cc898bfdc25941dd437e96b9a961843df4116dcb0f3ed31412d37a98493
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8493289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee203567cc45c4a8288b4650f2afc365f43eb01c42fac9f92c3063cacd70c332`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Thu, 28 Sep 2023 23:17:49 GMT
ENV NATS_SERVER=2.9.22
# Thu, 28 Sep 2023 23:17:51 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Thu, 28 Sep 2023 23:17:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Thu, 28 Sep 2023 23:17:51 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Thu, 28 Sep 2023 23:17:51 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Sep 2023 23:17:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 28 Sep 2023 23:17:51 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e6799cc112563f5bd57ccf66b5ae4e1acb9b0f9380f8ea5ff99bcdf394d87a`  
		Last Modified: Thu, 28 Sep 2023 23:18:48 GMT  
		Size: 5.6 MB (5592383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c2d8b97f2ee1947b9f1567d20195023a527212ead9b2fd1fc84c2c10f31282`  
		Last Modified: Thu, 28 Sep 2023 23:18:47 GMT  
		Size: 588.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b817a337dea1e3c1d94395fec370c3af29bd89dbb0149d57dd4b93c72cb9de`  
		Last Modified: Thu, 28 Sep 2023 23:18:47 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2.9.22-alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:974daab09263e17e09f36c429cdfa842c86e7f2a7f727e73ffa8d72a0c758228
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8735321 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:010bd6c9016879b86bd554939bd0f2be66a0aeb82d807fe7288519980f99879d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 02:05:37 GMT
ENV NATS_SERVER=2.9.22
# Fri, 29 Sep 2023 02:05:39 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='811e5a3c8187d937a753f182bd5ae2035c91604bda11a3b11023e5eea0504c41' ;; 		armhf) natsArch='arm6'; sha256='4d6f2f8ee9faf43de9fed5b43a0a5db836ad81797146065777b06a59f90cf1b0' ;; 		armv7) natsArch='arm7'; sha256='b8c83cd825b05d8d0610fc9352804fe810ae6bd9d8f0d814a39b0f152ec2ba79' ;; 		x86_64) natsArch='amd64'; sha256='9550278e34e94aebd410ec401bc145d3538e430ec2a40d5213fffdf9fdd49c27' ;; 		x86) natsArch='386'; sha256='a8ccdd37eac64b031ea96762d7f72a74445e9a708c0363549ba7e119fa79e52c' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Fri, 29 Sep 2023 02:05:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Fri, 29 Sep 2023 02:05:39 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Fri, 29 Sep 2023 02:05:39 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Sep 2023 02:05:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 02:05:39 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76dd4ee8336fd067d1c11dd90428c4b26bc79b3521db6ba65309bfd68fcfe6b3`  
		Last Modified: Fri, 29 Sep 2023 02:06:41 GMT  
		Size: 5.4 MB (5402492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7966cb0b0f8d4873987436d855fcb89402026d7357cf9799ebd7636393c7e55e`  
		Last Modified: Fri, 29 Sep 2023 02:06:40 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6944ab51200e30863838a2feffd3da50d117f096e4dec219cedaa5b62dff1249`  
		Last Modified: Fri, 29 Sep 2023 02:06:40 GMT  
		Size: 412.0 B  
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
$ docker pull nats@sha256:f1b504cc4d7a24a79cb3ec47cc7968cfaa56398af6f0a56c9b8f02c11e87e198
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.9.22-nanoserver` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:f5b7c7052aa1d091ef81f5cb49a31d3629b21ae5da1d018cae367e601bec0a6d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109791051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea9c2e90f2e383203bae762574ce31298840db6117cf2b43de8f73e2d8ad3e33`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:39:57 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 11 Oct 2023 03:39:58 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:39:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:39:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:40:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52fe086e7510cd640f31a862cc7ed0aae171d6591241c4eddfbeda3169a718b`  
		Last Modified: Wed, 11 Oct 2023 03:40:51 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6759c77fac899cf8e1905cc3ae8d80c50b89decfa9054624b3dd6f460076e9`  
		Last Modified: Wed, 11 Oct 2023 03:41:16 GMT  
		Size: 5.3 MB (5320077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7158fb411ea29a9e1b6be836314c1ba4116d7ff26e4f4b8fa471d96f745bf64`  
		Last Modified: Wed, 11 Oct 2023 03:41:15 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f7a5bb7f58543897c1f653f0aaf27d5cb41a6bc23e9d58aa4977e7c6a56b0f`  
		Last Modified: Wed, 11 Oct 2023 03:41:15 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ea4b403539176bffc7b5217fa85130223e1b0593d5535c7ee5bca120a4e471`  
		Last Modified: Wed, 11 Oct 2023 03:41:15 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff475aa742bc198c00f6e55c4f40c431e460d7272bb78e4a187a8476d7a8ac36`  
		Last Modified: Wed, 11 Oct 2023 03:41:15 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22-nanoserver-1809`

```console
$ docker pull nats@sha256:f1b504cc4d7a24a79cb3ec47cc7968cfaa56398af6f0a56c9b8f02c11e87e198
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.9.22-nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:f5b7c7052aa1d091ef81f5cb49a31d3629b21ae5da1d018cae367e601bec0a6d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109791051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea9c2e90f2e383203bae762574ce31298840db6117cf2b43de8f73e2d8ad3e33`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:39:57 GMT
RUN cmd /S /C #(nop) COPY file:393d7e944d1b6697a14f19f6cb9673d95da4e1a0fc9508b238325e94beebc857 in C:\nats-server.exe 
# Wed, 11 Oct 2023 03:39:58 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:39:59 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:39:59 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:40:00 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52fe086e7510cd640f31a862cc7ed0aae171d6591241c4eddfbeda3169a718b`  
		Last Modified: Wed, 11 Oct 2023 03:40:51 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc6759c77fac899cf8e1905cc3ae8d80c50b89decfa9054624b3dd6f460076e9`  
		Last Modified: Wed, 11 Oct 2023 03:41:16 GMT  
		Size: 5.3 MB (5320077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7158fb411ea29a9e1b6be836314c1ba4116d7ff26e4f4b8fa471d96f745bf64`  
		Last Modified: Wed, 11 Oct 2023 03:41:15 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f7a5bb7f58543897c1f653f0aaf27d5cb41a6bc23e9d58aa4977e7c6a56b0f`  
		Last Modified: Wed, 11 Oct 2023 03:41:15 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ea4b403539176bffc7b5217fa85130223e1b0593d5535c7ee5bca120a4e471`  
		Last Modified: Wed, 11 Oct 2023 03:41:15 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff475aa742bc198c00f6e55c4f40c431e460d7272bb78e4a187a8476d7a8ac36`  
		Last Modified: Wed, 11 Oct 2023 03:41:15 GMT  
		Size: 1.1 KB (1122 bytes)  
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
$ docker pull nats@sha256:a6425c9ec006beb738a167a459028fcca9f282e4e40d042284598a09b702a556
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.9.22-windowsservercore` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:045eb82cccf069cd433f0ea1844ca371c31bbb6a5100948a1c86b0847cc16775
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037669001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ece444de41a3389ace76622ea181809ffd86c614acbf5391eac86a523c8c1424`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:36:44 GMT
ENV NATS_SERVER=2.9.22
# Wed, 11 Oct 2023 03:36:45 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.22/nats-server-v2.9.22-windows-amd64.zip
# Wed, 11 Oct 2023 03:36:45 GMT
ENV NATS_SERVER_SHASUM=e91db73b02bd4dca3eb7a4bf32e29763450b08d593f73e87d0a6b70102dea0d4
# Wed, 11 Oct 2023 03:37:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Oct 2023 03:39:38 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 11 Oct 2023 03:39:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:39:40 GMT
EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:39:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:39:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d90788f0e55a4514b4130734c279ec44aca19b7b33db65a550c03f6c561ce4`  
		Last Modified: Wed, 11 Oct 2023 03:41:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa1528cb66af3af51f6a26e9a32fd00b8b7f1faa43e41bbe9f7b9077edd3ccf`  
		Last Modified: Wed, 11 Oct 2023 03:41:06 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9de9a1d29daf2f2518d42cbe7b08de42ee77f7b41f78e73437d193ea371bdd`  
		Last Modified: Wed, 11 Oct 2023 03:41:06 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea5bc356f3bfa68b3ca0a3129a9c4fd9d525eb71b58350c1ebd9780c851892`  
		Last Modified: Wed, 11 Oct 2023 03:41:06 GMT  
		Size: 450.5 KB (450507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb555481fabd89853d836bedfbe8efa7ee84b0e2cb440a37fb2a9ffbb96f7cfe`  
		Last Modified: Wed, 11 Oct 2023 03:41:05 GMT  
		Size: 5.6 MB (5614696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03163c07b0721c4a1d3270ccb7a7ace36fcee5c6550af64cb5c55b6d44ee772c`  
		Last Modified: Wed, 11 Oct 2023 03:41:04 GMT  
		Size: 2.0 KB (1966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fc000c6fcb389bf91057cc7a3f58c2dbf03e5bbe6aec78af7d96924c1176ae`  
		Last Modified: Wed, 11 Oct 2023 03:41:04 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5654a35313bcb88698d7d7db013197bd621a2cc8c3e6812ebc7000216ee451d9`  
		Last Modified: Wed, 11 Oct 2023 03:41:04 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caa0710f11b36a20354b2d9a9fd224b7c3fb6bc443f0350dfdf0655df236a92`  
		Last Modified: Wed, 11 Oct 2023 03:41:04 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:2.9.22-windowsservercore-1809`

```console
$ docker pull nats@sha256:a6425c9ec006beb738a167a459028fcca9f282e4e40d042284598a09b702a556
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:2.9.22-windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:045eb82cccf069cd433f0ea1844ca371c31bbb6a5100948a1c86b0847cc16775
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037669001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ece444de41a3389ace76622ea181809ffd86c614acbf5391eac86a523c8c1424`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:36:44 GMT
ENV NATS_SERVER=2.9.22
# Wed, 11 Oct 2023 03:36:45 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.22/nats-server-v2.9.22-windows-amd64.zip
# Wed, 11 Oct 2023 03:36:45 GMT
ENV NATS_SERVER_SHASUM=e91db73b02bd4dca3eb7a4bf32e29763450b08d593f73e87d0a6b70102dea0d4
# Wed, 11 Oct 2023 03:37:47 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Oct 2023 03:39:38 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 11 Oct 2023 03:39:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:39:40 GMT
EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:39:40 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:39:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d90788f0e55a4514b4130734c279ec44aca19b7b33db65a550c03f6c561ce4`  
		Last Modified: Wed, 11 Oct 2023 03:41:06 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa1528cb66af3af51f6a26e9a32fd00b8b7f1faa43e41bbe9f7b9077edd3ccf`  
		Last Modified: Wed, 11 Oct 2023 03:41:06 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e9de9a1d29daf2f2518d42cbe7b08de42ee77f7b41f78e73437d193ea371bdd`  
		Last Modified: Wed, 11 Oct 2023 03:41:06 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ea5bc356f3bfa68b3ca0a3129a9c4fd9d525eb71b58350c1ebd9780c851892`  
		Last Modified: Wed, 11 Oct 2023 03:41:06 GMT  
		Size: 450.5 KB (450507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb555481fabd89853d836bedfbe8efa7ee84b0e2cb440a37fb2a9ffbb96f7cfe`  
		Last Modified: Wed, 11 Oct 2023 03:41:05 GMT  
		Size: 5.6 MB (5614696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03163c07b0721c4a1d3270ccb7a7ace36fcee5c6550af64cb5c55b6d44ee772c`  
		Last Modified: Wed, 11 Oct 2023 03:41:04 GMT  
		Size: 2.0 KB (1966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fc000c6fcb389bf91057cc7a3f58c2dbf03e5bbe6aec78af7d96924c1176ae`  
		Last Modified: Wed, 11 Oct 2023 03:41:04 GMT  
		Size: 1.4 KB (1381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5654a35313bcb88698d7d7db013197bd621a2cc8c3e6812ebc7000216ee451d9`  
		Last Modified: Wed, 11 Oct 2023 03:41:04 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caa0710f11b36a20354b2d9a9fd224b7c3fb6bc443f0350dfdf0655df236a92`  
		Last Modified: Wed, 11 Oct 2023 03:41:04 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine`

```console
$ docker pull nats@sha256:c6d778a0df2aeeec2399f1e1ce558d7b65e70adc7ef5ca13f2cf06b1f7654a08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine` - linux; amd64

```console
$ docker pull nats@sha256:d6a47f89f52342be07d213d493e0b71a80fc94ccc19edc9c8b17169e8d887fbe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9494811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18e20b07c9925b57a0846b64bffdab236ff0d02728bea2661094cb2f1088d89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:20:15 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:20:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:20:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:20:17 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:20:17 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:20:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:20:17 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793ee3203ddeae4265feedfeeb0176c5d046487786e6430ec414b466b7342687`  
		Last Modified: Mon, 09 Oct 2023 23:21:01 GMT  
		Size: 6.1 MB (6091846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0dd902fefeb39726cbb9025e935fabe591af4d39f448ddad514c70eb56a6002`  
		Last Modified: Mon, 09 Oct 2023 23:21:00 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7a1bcf5bcb5ad0317a82f43795966d7b0cf297054e112bc548fe8d0c881df9`  
		Last Modified: Mon, 09 Oct 2023 23:21:00 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v6

```console
$ docker pull nats@sha256:6d9d5fd5f91a7c3e45e2cac23df6f50393e2024ea69495d9233df8ba9503bdc8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8958058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11708ece1d9ad1b7baf64c1f3c5e3b7a38ef5d66e87c24ba859eb6272bc2694f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:49:18 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:49:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:49:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:49:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:49:21 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dece2e91316626c2aeb73fab796c9095ba11a38f43e17e03f3cea33bada9941e`  
		Last Modified: Mon, 09 Oct 2023 23:49:58 GMT  
		Size: 5.8 MB (5811761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0164ce1b0fe0ce335f0348dbf1ef83dca670a9bb6c3036586e38f45c257ab3`  
		Last Modified: Mon, 09 Oct 2023 23:49:57 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a6185289b767b3266aeff451a57e88263f01cbb1544b137dd118ad2aa87d88`  
		Last Modified: Mon, 09 Oct 2023 23:49:57 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm variant v7

```console
$ docker pull nats@sha256:56973c518df167ff13997d599dd6f0f488eb2a00380d161395d001cbd82ef4f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8701812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c71794277a3ea4fd3358f79bd24730e7bff545f116dbae54391ff86f7b5ba91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:57:29 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:57:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:57:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:57:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:57:31 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:57:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1577c013973725bb512b6e87006f323da7dece18dc8d5cddf516ac8ac1bd3690`  
		Last Modified: Mon, 09 Oct 2023 23:58:15 GMT  
		Size: 5.8 MB (5800912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2989475d4fcb37e49592f48904864c46ac84f25ca502bbddacc54bddf27ec9a3`  
		Last Modified: Mon, 09 Oct 2023 23:58:14 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dca18857ae02bbc23b7a6d389a1036fd7822d30861d1f065a1fce1b2662745e`  
		Last Modified: Mon, 09 Oct 2023 23:58:14 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a1cc118cb20105a3d28409f6f0134779e37d691cdfc8340e26aa21bf5c1fcecb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8999244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c690558bd2217d60e3ef1f45a02405b0c52118f1c91dda8b42c091696af68306`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:39:44 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:39:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:39:47 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:39:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e016e40994857a38606186dc8f2061ac54ed621273f59128aa5c6d060fb22`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 5.7 MB (5666417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15cff88ae624a30801728dd1b20bb84f6e871846c236cf2613ec7c7fb6008f1`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68049c030ad10066e6a3a63f9d02398f98a4b8bf2104c8d22adb9aed0ff83e1`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:alpine3.18`

```console
$ docker pull nats@sha256:c6d778a0df2aeeec2399f1e1ce558d7b65e70adc7ef5ca13f2cf06b1f7654a08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:alpine3.18` - linux; amd64

```console
$ docker pull nats@sha256:d6a47f89f52342be07d213d493e0b71a80fc94ccc19edc9c8b17169e8d887fbe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.5 MB (9494811 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18e20b07c9925b57a0846b64bffdab236ff0d02728bea2661094cb2f1088d89`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:20:15 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:20:17 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:20:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:20:17 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:20:17 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:20:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:20:17 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793ee3203ddeae4265feedfeeb0176c5d046487786e6430ec414b466b7342687`  
		Last Modified: Mon, 09 Oct 2023 23:21:01 GMT  
		Size: 6.1 MB (6091846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0dd902fefeb39726cbb9025e935fabe591af4d39f448ddad514c70eb56a6002`  
		Last Modified: Mon, 09 Oct 2023 23:21:00 GMT  
		Size: 586.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c7a1bcf5bcb5ad0317a82f43795966d7b0cf297054e112bc548fe8d0c881df9`  
		Last Modified: Mon, 09 Oct 2023 23:21:00 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v6

```console
$ docker pull nats@sha256:6d9d5fd5f91a7c3e45e2cac23df6f50393e2024ea69495d9233df8ba9503bdc8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8958058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11708ece1d9ad1b7baf64c1f3c5e3b7a38ef5d66e87c24ba859eb6272bc2694f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:49:18 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:49:21 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:49:21 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:49:21 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:49:21 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:49:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:49:21 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dece2e91316626c2aeb73fab796c9095ba11a38f43e17e03f3cea33bada9941e`  
		Last Modified: Mon, 09 Oct 2023 23:49:58 GMT  
		Size: 5.8 MB (5811761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0164ce1b0fe0ce335f0348dbf1ef83dca670a9bb6c3036586e38f45c257ab3`  
		Last Modified: Mon, 09 Oct 2023 23:49:57 GMT  
		Size: 587.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a6185289b767b3266aeff451a57e88263f01cbb1544b137dd118ad2aa87d88`  
		Last Modified: Mon, 09 Oct 2023 23:49:57 GMT  
		Size: 419.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm variant v7

```console
$ docker pull nats@sha256:56973c518df167ff13997d599dd6f0f488eb2a00380d161395d001cbd82ef4f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.7 MB (8701812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c71794277a3ea4fd3358f79bd24730e7bff545f116dbae54391ff86f7b5ba91`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:57:29 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:57:31 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:57:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:57:31 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:57:31 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:57:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:57:32 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1577c013973725bb512b6e87006f323da7dece18dc8d5cddf516ac8ac1bd3690`  
		Last Modified: Mon, 09 Oct 2023 23:58:15 GMT  
		Size: 5.8 MB (5800912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2989475d4fcb37e49592f48904864c46ac84f25ca502bbddacc54bddf27ec9a3`  
		Last Modified: Mon, 09 Oct 2023 23:58:14 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dca18857ae02bbc23b7a6d389a1036fd7822d30861d1f065a1fce1b2662745e`  
		Last Modified: Mon, 09 Oct 2023 23:58:14 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:alpine3.18` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a1cc118cb20105a3d28409f6f0134779e37d691cdfc8340e26aa21bf5c1fcecb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8999244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c690558bd2217d60e3ef1f45a02405b0c52118f1c91dda8b42c091696af68306`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["nats-server","--config","\/etc\/nats\/nats-server.conf"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Mon, 09 Oct 2023 23:39:44 GMT
ENV NATS_SERVER=2.10.2
# Mon, 09 Oct 2023 23:39:46 GMT
RUN set -eux; 	apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		aarch64) natsArch='arm64'; sha256='26b3816709136a8d061e5147cfb217abb577d1fd79e08689417c9b0fa2806533' ;; 		armhf) natsArch='arm6'; sha256='189131c2b890446d88b508cc7e8aa937c38fef81dbd3f4b4d3d205af41edb5ab' ;; 		armv7) natsArch='arm7'; sha256='33374ac52531ac0a8c57c2f111d098eb99c42120fedfad57317817e6d48d70d2' ;; 		x86_64) natsArch='amd64'; sha256='8929b053d2dca2b62756982951c51147b69be984b55a7a850affa86a66c6bfc9' ;; 		x86) natsArch='386'; sha256='b11c6bded174332b3fc88ac40c3632448d58e8d58dc92551d9655407ce0107e8' ;; 		*) echo >&2 "error: $apkArch is not supported!"; exit 1 ;; 	esac; 		wget -O nats-server.tar.gz "https://github.com/nats-io/nats-server/releases/download/v${NATS_SERVER}/nats-server-v${NATS_SERVER}-linux-${natsArch}.tar.gz"; 	echo "${sha256} *nats-server.tar.gz" | sha256sum -c -; 		apk add --no-cache ca-certificates tzdata; 		tar -xf nats-server.tar.gz; 	rm nats-server.tar.gz; 	mv "nats-server-v${NATS_SERVER}-linux-${natsArch}/nats-server" /usr/local/bin; 	rm -rf "nats-server-v${NATS_SERVER}-linux-${natsArch}";
# Mon, 09 Oct 2023 23:39:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /etc/nats/nats-server.conf 
# Mon, 09 Oct 2023 23:39:47 GMT
COPY file:b2810cc282a84164c4e1e5f77556bd78260283c00b329045f3f64a63f71e3570 in /usr/local/bin 
# Mon, 09 Oct 2023 23:39:47 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:39:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Oct 2023 23:39:47 GMT
CMD ["nats-server" "--config" "/etc/nats/nats-server.conf"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149e016e40994857a38606186dc8f2061ac54ed621273f59128aa5c6d060fb22`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 5.7 MB (5666417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15cff88ae624a30801728dd1b20bb84f6e871846c236cf2613ec7c7fb6008f1`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 584.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68049c030ad10066e6a3a63f9d02398f98a4b8bf2104c8d22adb9aed0ff83e1`  
		Last Modified: Mon, 09 Oct 2023 23:40:22 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:latest`

```console
$ docker pull nats@sha256:00950ae452fd32e036bb1de4eca8cb02902ad876425626cf4b752f44057e4b06
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
	-	windows version 10.0.17763.4974; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:7be2e854c9542ad2146d9baadede0f2e3d520d9ffc8b9ef24078852362d95c5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5469432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d633df072e1a202141ac94a984750c13337fede7f772b34400dc99a9285cd99`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:a7de81fdc98e0908f1fbfd4b16f2eeac146932aac03b4a109a89f93b3efbfc58 in /nats-server 
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:20:31 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:20:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:20:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:494ad87960e9c491e7d14b1b9a5ca82020e4b968c60a0f3bffece88c8cee4831`  
		Last Modified: Sun, 08 Oct 2023 12:45:05 GMT  
		Size: 5.5 MB (5468923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d4a6b4c3024603d5932b75b727d2b94f22a490f5326099a6112bf261dfebc5`  
		Last Modified: Mon, 09 Oct 2023 23:21:26 GMT  
		Size: 509.0 B  
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
$ docker pull nats@sha256:4311525539cb532e2215a0f0e6a97e456bf100aecae9df633068dce84725d3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5189188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b74620a2c8b938dece7aba41cf3db596039ac4579268f2083d879dc0338e3d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:78bf14fdba87d3f994b59ec64fa5f813ff988f0f91e4929c7aaf33d206d6e4e2 in /nats-server 
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:49:30 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:49:30 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:49:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:541bfb4a7866a6fb7234b9fb133b37cc8a1fff7bcf10779570793f66bfa36cc5`  
		Last Modified: Mon, 09 Oct 2023 23:50:25 GMT  
		Size: 5.2 MB (5188681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e9969a228338f491f74c367e86a77a512ae318604d924fa624ef4e9b944a62`  
		Last Modified: Mon, 09 Oct 2023 23:50:24 GMT  
		Size: 507.0 B  
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
$ docker pull nats@sha256:72a048e9abb13148a5588dd1f556af5cf11e91369fd856d21e1b981e2f0f6aec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3f7200638809e9d2ec5971ab53b5a84b4413d7fce360c58f1d7381d739555e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:dfba40eb121bd5821909fe10c59b498aec418c7224d18a7961e71444dc375765 in /nats-server 
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:57:51 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c24b02c85cdfcd5bdce9a848ef068ff9e9535a6287fb7a00eb8e39b357c54ad0`  
		Last Modified: Mon, 09 Oct 2023 23:58:40 GMT  
		Size: 5.2 MB (5177978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d844de696d0e40f4aff106f51467e397619526062047fe60f4b692adda3bd736`  
		Last Modified: Mon, 09 Oct 2023 23:58:39 GMT  
		Size: 507.0 B  
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
$ docker pull nats@sha256:4b167dea0c683971c7d06db669fbdebf2a8b3c01cb4d229bf5204c8fc6cab7e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5042145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966bdbd5f41b922365e541cf6121d6cf76a4ddb1f9c111e010656f7041d50c1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:c0f257aca3b8b7405bb5549a368de7ae62c806fe4e75e189b405a7ce1f65fa4b in /nats-server 
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:39:55 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:39:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:39:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12032ad6ebd443b7c142112d1df3d64b3deb3a403e0a99764593e5fe7843781b`  
		Last Modified: Mon, 09 Oct 2023 23:40:46 GMT  
		Size: 5.0 MB (5041638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7d34c174da06f5ab9c869a0197e492849a0d80fbf8f038f93e9e1ac634d1f7`  
		Last Modified: Mon, 09 Oct 2023 23:40:45 GMT  
		Size: 507.0 B  
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

### `nats:latest` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:d0a9a23bc5e727b8b8db67f5a02c6be5d0dfba5700152d11e56457862713e866
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110053852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f669b1f92bc1e89b2470de199627f90a4496308a2cd8c5f8bfd06b52ecf39a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:36:34 GMT
RUN cmd /S /C #(nop) COPY file:56de93ec6afaefd5f19b9effd4409842fdfa695280fb05da230b1d12a03db7bb in C:\nats-server.exe 
# Wed, 11 Oct 2023 03:36:35 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52fe086e7510cd640f31a862cc7ed0aae171d6591241c4eddfbeda3169a718b`  
		Last Modified: Wed, 11 Oct 2023 03:40:51 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f15b99379f9a65c4a40e86d7f09407cf716ae5cdd5ec3fdfbcd609fceb69f5`  
		Last Modified: Wed, 11 Oct 2023 03:40:50 GMT  
		Size: 5.6 MB (5582847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3574203dd8b3d01c5d1979302e56d73e3c604318c215efb12f98e667c80879`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937e84807bea241751a5e003bbf2cca02d1a37306e3cd7d17e260322cebb9e70`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fde0249533da9dfa2f6b077b43c2290316223ac025f271a8ba383f1136ff00`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee3b7476b8b4cb6aa82268271e5e2971d380d8da227366182b80abcfacc961`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:linux`

```console
$ docker pull nats@sha256:6a7739943a7360813f70dba186b72c6aba2163f2809fce7672cc3657b62043ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:7be2e854c9542ad2146d9baadede0f2e3d520d9ffc8b9ef24078852362d95c5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5469432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d633df072e1a202141ac94a984750c13337fede7f772b34400dc99a9285cd99`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:a7de81fdc98e0908f1fbfd4b16f2eeac146932aac03b4a109a89f93b3efbfc58 in /nats-server 
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:20:31 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:20:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:20:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:494ad87960e9c491e7d14b1b9a5ca82020e4b968c60a0f3bffece88c8cee4831`  
		Last Modified: Sun, 08 Oct 2023 12:45:05 GMT  
		Size: 5.5 MB (5468923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d4a6b4c3024603d5932b75b727d2b94f22a490f5326099a6112bf261dfebc5`  
		Last Modified: Mon, 09 Oct 2023 23:21:26 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:4311525539cb532e2215a0f0e6a97e456bf100aecae9df633068dce84725d3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5189188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b74620a2c8b938dece7aba41cf3db596039ac4579268f2083d879dc0338e3d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:78bf14fdba87d3f994b59ec64fa5f813ff988f0f91e4929c7aaf33d206d6e4e2 in /nats-server 
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:49:30 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:49:30 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:49:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:541bfb4a7866a6fb7234b9fb133b37cc8a1fff7bcf10779570793f66bfa36cc5`  
		Last Modified: Mon, 09 Oct 2023 23:50:25 GMT  
		Size: 5.2 MB (5188681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e9969a228338f491f74c367e86a77a512ae318604d924fa624ef4e9b944a62`  
		Last Modified: Mon, 09 Oct 2023 23:50:24 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:72a048e9abb13148a5588dd1f556af5cf11e91369fd856d21e1b981e2f0f6aec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3f7200638809e9d2ec5971ab53b5a84b4413d7fce360c58f1d7381d739555e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:dfba40eb121bd5821909fe10c59b498aec418c7224d18a7961e71444dc375765 in /nats-server 
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:57:51 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c24b02c85cdfcd5bdce9a848ef068ff9e9535a6287fb7a00eb8e39b357c54ad0`  
		Last Modified: Mon, 09 Oct 2023 23:58:40 GMT  
		Size: 5.2 MB (5177978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d844de696d0e40f4aff106f51467e397619526062047fe60f4b692adda3bd736`  
		Last Modified: Mon, 09 Oct 2023 23:58:39 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:4b167dea0c683971c7d06db669fbdebf2a8b3c01cb4d229bf5204c8fc6cab7e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5042145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966bdbd5f41b922365e541cf6121d6cf76a4ddb1f9c111e010656f7041d50c1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:c0f257aca3b8b7405bb5549a368de7ae62c806fe4e75e189b405a7ce1f65fa4b in /nats-server 
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:39:55 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:39:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:39:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12032ad6ebd443b7c142112d1df3d64b3deb3a403e0a99764593e5fe7843781b`  
		Last Modified: Mon, 09 Oct 2023 23:40:46 GMT  
		Size: 5.0 MB (5041638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7d34c174da06f5ab9c869a0197e492849a0d80fbf8f038f93e9e1ac634d1f7`  
		Last Modified: Mon, 09 Oct 2023 23:40:45 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver`

```console
$ docker pull nats@sha256:d2017f7731ec6420f52e2633c4567934fc67c6b1466820f14cf57a737f77433c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:nanoserver` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:d0a9a23bc5e727b8b8db67f5a02c6be5d0dfba5700152d11e56457862713e866
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110053852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f669b1f92bc1e89b2470de199627f90a4496308a2cd8c5f8bfd06b52ecf39a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:36:34 GMT
RUN cmd /S /C #(nop) COPY file:56de93ec6afaefd5f19b9effd4409842fdfa695280fb05da230b1d12a03db7bb in C:\nats-server.exe 
# Wed, 11 Oct 2023 03:36:35 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52fe086e7510cd640f31a862cc7ed0aae171d6591241c4eddfbeda3169a718b`  
		Last Modified: Wed, 11 Oct 2023 03:40:51 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f15b99379f9a65c4a40e86d7f09407cf716ae5cdd5ec3fdfbcd609fceb69f5`  
		Last Modified: Wed, 11 Oct 2023 03:40:50 GMT  
		Size: 5.6 MB (5582847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3574203dd8b3d01c5d1979302e56d73e3c604318c215efb12f98e667c80879`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937e84807bea241751a5e003bbf2cca02d1a37306e3cd7d17e260322cebb9e70`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fde0249533da9dfa2f6b077b43c2290316223ac025f271a8ba383f1136ff00`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee3b7476b8b4cb6aa82268271e5e2971d380d8da227366182b80abcfacc961`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:nanoserver-1809`

```console
$ docker pull nats@sha256:d2017f7731ec6420f52e2633c4567934fc67c6b1466820f14cf57a737f77433c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:d0a9a23bc5e727b8b8db67f5a02c6be5d0dfba5700152d11e56457862713e866
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110053852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f669b1f92bc1e89b2470de199627f90a4496308a2cd8c5f8bfd06b52ecf39a6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 03:36:33 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:36:34 GMT
RUN cmd /S /C #(nop) COPY file:56de93ec6afaefd5f19b9effd4409842fdfa695280fb05da230b1d12a03db7bb in C:\nats-server.exe 
# Wed, 11 Oct 2023 03:36:35 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:36 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:37 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52fe086e7510cd640f31a862cc7ed0aae171d6591241c4eddfbeda3169a718b`  
		Last Modified: Wed, 11 Oct 2023 03:40:51 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f15b99379f9a65c4a40e86d7f09407cf716ae5cdd5ec3fdfbcd609fceb69f5`  
		Last Modified: Wed, 11 Oct 2023 03:40:50 GMT  
		Size: 5.6 MB (5582847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3574203dd8b3d01c5d1979302e56d73e3c604318c215efb12f98e667c80879`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.8 KB (1784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:937e84807bea241751a5e003bbf2cca02d1a37306e3cd7d17e260322cebb9e70`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fde0249533da9dfa2f6b077b43c2290316223ac025f271a8ba383f1136ff00`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44ee3b7476b8b4cb6aa82268271e5e2971d380d8da227366182b80abcfacc961`  
		Last Modified: Wed, 11 Oct 2023 03:40:49 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:scratch`

```console
$ docker pull nats@sha256:6a7739943a7360813f70dba186b72c6aba2163f2809fce7672cc3657b62043ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:7be2e854c9542ad2146d9baadede0f2e3d520d9ffc8b9ef24078852362d95c5d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5469432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d633df072e1a202141ac94a984750c13337fede7f772b34400dc99a9285cd99`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:a7de81fdc98e0908f1fbfd4b16f2eeac146932aac03b4a109a89f93b3efbfc58 in /nats-server 
# Mon, 09 Oct 2023 23:20:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:20:31 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:20:31 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:20:31 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:494ad87960e9c491e7d14b1b9a5ca82020e4b968c60a0f3bffece88c8cee4831`  
		Last Modified: Sun, 08 Oct 2023 12:45:05 GMT  
		Size: 5.5 MB (5468923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d4a6b4c3024603d5932b75b727d2b94f22a490f5326099a6112bf261dfebc5`  
		Last Modified: Mon, 09 Oct 2023 23:21:26 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:4311525539cb532e2215a0f0e6a97e456bf100aecae9df633068dce84725d3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5189188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29b74620a2c8b938dece7aba41cf3db596039ac4579268f2083d879dc0338e3d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:78bf14fdba87d3f994b59ec64fa5f813ff988f0f91e4929c7aaf33d206d6e4e2 in /nats-server 
# Mon, 09 Oct 2023 23:49:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:49:30 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:49:30 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:49:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:541bfb4a7866a6fb7234b9fb133b37cc8a1fff7bcf10779570793f66bfa36cc5`  
		Last Modified: Mon, 09 Oct 2023 23:50:25 GMT  
		Size: 5.2 MB (5188681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e9969a228338f491f74c367e86a77a512ae318604d924fa624ef4e9b944a62`  
		Last Modified: Mon, 09 Oct 2023 23:50:24 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:72a048e9abb13148a5588dd1f556af5cf11e91369fd856d21e1b981e2f0f6aec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a3f7200638809e9d2ec5971ab53b5a84b4413d7fce360c58f1d7381d739555e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:dfba40eb121bd5821909fe10c59b498aec418c7224d18a7961e71444dc375765 in /nats-server 
# Mon, 09 Oct 2023 23:57:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:57:51 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:57:51 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:57:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c24b02c85cdfcd5bdce9a848ef068ff9e9535a6287fb7a00eb8e39b357c54ad0`  
		Last Modified: Mon, 09 Oct 2023 23:58:40 GMT  
		Size: 5.2 MB (5177978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d844de696d0e40f4aff106f51467e397619526062047fe60f4b692adda3bd736`  
		Last Modified: Mon, 09 Oct 2023 23:58:39 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:4b167dea0c683971c7d06db669fbdebf2a8b3c01cb4d229bf5204c8fc6cab7e2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5042145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:966bdbd5f41b922365e541cf6121d6cf76a4ddb1f9c111e010656f7041d50c1f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:c0f257aca3b8b7405bb5549a368de7ae62c806fe4e75e189b405a7ce1f65fa4b in /nats-server 
# Mon, 09 Oct 2023 23:39:55 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Mon, 09 Oct 2023 23:39:55 GMT
EXPOSE 4222 6222 8222
# Mon, 09 Oct 2023 23:39:55 GMT
ENTRYPOINT ["/nats-server"]
# Mon, 09 Oct 2023 23:39:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:12032ad6ebd443b7c142112d1df3d64b3deb3a403e0a99764593e5fe7843781b`  
		Last Modified: Mon, 09 Oct 2023 23:40:46 GMT  
		Size: 5.0 MB (5041638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7d34c174da06f5ab9c869a0197e492849a0d80fbf8f038f93e9e1ac634d1f7`  
		Last Modified: Mon, 09 Oct 2023 23:40:45 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore`

```console
$ docker pull nats@sha256:8dbf04badbb41fc71c6e2880ff3bbbfd4b117d6abced349307322c18e014c117
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:windowsservercore` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:059aab4410ed4545cb5ce2d8dd236f0b5c3568341a60c48bd5a1cce6a34ad97f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037905706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d15e9ed22631845e0f6ab08ef7c67bfb34f20ef808833c7243bd894a1978af84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:32:18 GMT
ENV NATS_SERVER=2.10.2
# Wed, 11 Oct 2023 03:32:19 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.2/nats-server-v2.10.2-windows-amd64.zip
# Wed, 11 Oct 2023 03:32:21 GMT
ENV NATS_SERVER_SHASUM=ce8eed07736cc6e008b0d26808ec0cae5871a419d8e38b020cfd121d0f88b935
# Wed, 11 Oct 2023 03:34:22 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Oct 2023 03:36:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 11 Oct 2023 03:36:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:12 GMT
EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362b60e14057a139612c4649868ad03cdc62c387c1b84d4908aa5908f87e20ff`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64517fb064d3b69109b8e9f259256e0ef3f0adc49276790fb0e5fb4ece78cfc`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2263f3dafd6f25001f85eb3b171366a90f088823c95e5a559b5aa62ee251809`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bc429c4e89ff3ab7798f0ae3347e48b4979ea71a3740c2c0056936bc378ec0`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 438.0 KB (437960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f9316683d04ebbebf399d13c5de2e8c262b352dd1f08c6fbb0cf7911187aeb`  
		Last Modified: Wed, 11 Oct 2023 03:40:32 GMT  
		Size: 5.9 MB (5863943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd7967ce50710cf0aefd72c029cd070a7c29865152d227e1def2edb5d0f4365`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123be7b303544a1edb1cf1a28202059f984c7050377fe77230633e9f80a9658c`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218eeb362e2a56ad3bc9c71e196900056c5c067cc3cef638e395caa8dd31ff20`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f857db4d13bfffe59dac02cd3f605fb4ecaca8297626b1dbe54c6e27c82bb5`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `nats:windowsservercore-1809`

```console
$ docker pull nats@sha256:8dbf04badbb41fc71c6e2880ff3bbbfd4b117d6abced349307322c18e014c117
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `nats:windowsservercore-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull nats@sha256:059aab4410ed4545cb5ce2d8dd236f0b5c3568341a60c48bd5a1cce6a34ad97f
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (2037905706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d15e9ed22631845e0f6ab08ef7c67bfb34f20ef808833c7243bd894a1978af84`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 08 Jun 2023 12:58:24 GMT
RUN Apply image 10.0.17763.4499
# Mon, 02 Oct 2023 08:29:38 GMT
RUN Install update 10.0.17763.4974
# Wed, 11 Oct 2023 02:58:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Oct 2023 03:32:17 GMT
ENV NATS_DOCKERIZED=1
# Wed, 11 Oct 2023 03:32:18 GMT
ENV NATS_SERVER=2.10.2
# Wed, 11 Oct 2023 03:32:19 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.10.2/nats-server-v2.10.2-windows-amd64.zip
# Wed, 11 Oct 2023 03:32:21 GMT
ENV NATS_SERVER_SHASUM=ce8eed07736cc6e008b0d26808ec0cae5871a419d8e38b020cfd121d0f88b935
# Wed, 11 Oct 2023 03:34:22 GMT
RUN Set-PSDebug -Trace 2
# Wed, 11 Oct 2023 03:36:11 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 11 Oct 2023 03:36:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 11 Oct 2023 03:36:12 GMT
EXPOSE 4222 6222 8222
# Wed, 11 Oct 2023 03:36:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 11 Oct 2023 03:36:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:c9226d61d3bdbf9f09821b32f5878623b8daaa5fb4f875cb63c199f87a26d57e`  
		Last Modified: Tue, 13 Jun 2023 18:25:35 GMT  
		Size: 1.7 GB (1650620357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af2bcb37edaec1dd87fc4a6f7c9129ca37bf1f91b65eb365ba9d4c70473beea`  
		Last Modified: Tue, 10 Oct 2023 17:51:10 GMT  
		Size: 381.0 MB (380970130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a4919cd870c32d33d8113b108e3e6ea2391bbbc70b2cf7e9febeeee307b1a4`  
		Last Modified: Wed, 11 Oct 2023 03:40:35 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce27dbaad0cf1a29b13da65c8ec2c9e6b42aaf192bb7138ab6c5b740dbd77b05`  
		Last Modified: Wed, 11 Oct 2023 03:40:34 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:362b60e14057a139612c4649868ad03cdc62c387c1b84d4908aa5908f87e20ff`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64517fb064d3b69109b8e9f259256e0ef3f0adc49276790fb0e5fb4ece78cfc`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2263f3dafd6f25001f85eb3b171366a90f088823c95e5a559b5aa62ee251809`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bc429c4e89ff3ab7798f0ae3347e48b4979ea71a3740c2c0056936bc378ec0`  
		Last Modified: Wed, 11 Oct 2023 03:40:33 GMT  
		Size: 438.0 KB (437960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49f9316683d04ebbebf399d13c5de2e8c262b352dd1f08c6fbb0cf7911187aeb`  
		Last Modified: Wed, 11 Oct 2023 03:40:32 GMT  
		Size: 5.9 MB (5863943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd7967ce50710cf0aefd72c029cd070a7c29865152d227e1def2edb5d0f4365`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 2.0 KB (1961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:123be7b303544a1edb1cf1a28202059f984c7050377fe77230633e9f80a9658c`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218eeb362e2a56ad3bc9c71e196900056c5c067cc3cef638e395caa8dd31ff20`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f857db4d13bfffe59dac02cd3f605fb4ecaca8297626b1dbe54c6e27c82bb5`  
		Last Modified: Wed, 11 Oct 2023 03:40:31 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
