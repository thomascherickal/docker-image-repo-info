## `nats:latest`

```console
$ docker pull nats@sha256:8f0cdcbc4c3597443fce869e75a759edb0d5a93fe98078f470a43204a6d7a729
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3287; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:796298f636925dedbbdfa537f42423dffd3a69b70c3a9bf4fd0982886a4b745d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4591595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:842c053e15bdb38e697668b1f0721313203f7c2297eb6d79000f20858dc97854`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 27 May 2022 00:38:26 GMT
COPY file:c866dea678e8cec7cbd0798a1dbdefc45e992d9df374709f6000bac517589a1b in /nats-server 
# Fri, 27 May 2022 00:38:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 27 May 2022 00:38:27 GMT
EXPOSE 4222 6222 8222
# Fri, 27 May 2022 00:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 27 May 2022 00:38:27 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 27 May 2022 00:38:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5e5797f39fa0527a3dd0a137353b40f97c71134e7eb38373d9791c5f1392885b`  
		Last Modified: Fri, 27 May 2022 00:39:15 GMT  
		Size: 4.6 MB (4591087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c3b732adf61929b0b23ca08934cd89923e9cd9d7061544e76bbce57a9fa1e4`  
		Last Modified: Fri, 27 May 2022 00:39:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:e0c28a95cdf6dd8a566d5c2394d09e6141dffb9107fe49f9385d6f19048bd955
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4245827 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cef47371f249bc862484ca7bd4dde2d7f77dc41bcb49cc49cceb17dfb2d4471f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:8de8b0cf8e6edf54e413c112cd66aed537abed387a26ba749a9293d43cdf6594 in /nats-server 
# Thu, 11 Aug 2022 01:12:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 11 Aug 2022 01:12:06 GMT
EXPOSE 4222 6222 8222
# Thu, 11 Aug 2022 01:12:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 11 Aug 2022 01:12:06 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 11 Aug 2022 01:12:06 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:770fa9c168613edbe7aa7007d2cf8492c6570efc1ddab217fa32772c6b72dd48`  
		Last Modified: Thu, 26 May 2022 23:58:21 GMT  
		Size: 4.2 MB (4245317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde47aae170f9c7e50b7bbea164ec0e0d02b9c05b603e7f7554e163183c02cd9`  
		Last Modified: Thu, 11 Aug 2022 01:13:30 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:453c8fea5d37abc60f034f80bdb668a48c8e4f0900fce8b55fdb6ae7f2908d07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4242795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:508b00336aa0fc72bd1c3d33e5f447d1411e47221dfa1fa6085d6986b27045d7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2841d6664b8897473f39b595b9aa4b28e749f587dc1afa4a0027ae507f37ee1f in /nats-server 
# Tue, 09 Aug 2022 22:36:22 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 09 Aug 2022 22:36:22 GMT
EXPOSE 4222 6222 8222
# Tue, 09 Aug 2022 22:36:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 09 Aug 2022 22:36:23 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 09 Aug 2022 22:36:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f533e6e439ee51f1cf94458f821a20ed162b542d356340957091882ad881d5c1`  
		Last Modified: Fri, 27 May 2022 00:28:16 GMT  
		Size: 4.2 MB (4242287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274ba9becbe1086958e9d56ab9452ec01f7fad6e3e68a34c49f1f299a5eab1ac`  
		Last Modified: Tue, 09 Aug 2022 22:38:14 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:87b1afbd78a75ee48cb6b37a8522bbb01f5e9b5047b095b16cc4f241774a48d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4227885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bce5ae01237736c7e0447d8cd1b2dbe252eab3ab5ac3b05d98b646b2575cee`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 26 May 2022 23:53:56 GMT
COPY file:2dbd94c6c11f89ceba3241f1efe469d0a06f0aae91abb77f3d79756676d0be57 in /nats-server 
# Thu, 26 May 2022 23:53:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 26 May 2022 23:53:57 GMT
EXPOSE 4222 6222 8222
# Thu, 26 May 2022 23:53:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 26 May 2022 23:53:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 26 May 2022 23:54:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c74770da2ea808362085edd6dead652091b3e3d34c1e32c50015a6a5bb36c02`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 4.2 MB (4227378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988af7458b707048622e497d5ae818b77d3a24ed0295a7897ced8f003179f7f9`  
		Last Modified: Thu, 26 May 2022 23:55:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.3287; amd64

```console
$ docker pull nats@sha256:1cedf48ffc2053a99d48b9d25a25aafa92106fbeeb92fe41aeb237d72e722664
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.8 MB (107843136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68f300c81963c2298e1d161245bcc24caccb02bc76fa1f665acbb465b70ff518`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 06 Aug 2022 18:08:38 GMT
RUN Apply image 10.0.17763.3287
# Wed, 10 Aug 2022 15:30:21 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Aug 2022 15:30:22 GMT
RUN cmd /S /C #(nop) COPY file:88c957e774978b3592c1072a38fbf2d578a30b42e89604bf16828cccd9f86b17 in C:\nats-server.exe 
# Wed, 10 Aug 2022 15:30:23 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Wed, 10 Aug 2022 15:30:24 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 10 Aug 2022 15:30:25 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5c9d6483dab113d2d9b50fdf3156622aa2ec3d6faaed5664d15a5568032d1714`  
		Size: 103.2 MB (103204200 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a5df16ce106b092b5399678da04735c18584e4f99ea301691eb433072953e9a`  
		Last Modified: Wed, 10 Aug 2022 15:31:14 GMT  
		Size: 1.0 KB (1025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0da7ec45038de57bb4ae201762e54193e71ffc21892b700c1942bd3b85a10ac`  
		Last Modified: Wed, 10 Aug 2022 15:31:13 GMT  
		Size: 4.6 MB (4633133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d561d8a7d904db478c9c1e66aae419bb3d5333483d2d9f39f39e7bc62c02c56d`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.7 KB (1653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e9538ca1cb2f704590a6fdaaef3b512b5ac93696534421be5f67017ffe8b9`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660c54f5d2b9ddc91667f920a6f2103c75527be0b892d65aa55dd5bfa8afd3fe`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.1 KB (1056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9356123a2a1af8afcf36b9979e254c522e7759fba29e96837a9d80c3a723f12c`  
		Last Modified: Wed, 10 Aug 2022 15:31:12 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
