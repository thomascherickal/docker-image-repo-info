## `nats:latest`

```console
$ docker pull nats@sha256:fd418d35ede5219e5d6e63eff16832de5a456e2463ab62c43092b054b88d065c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2237; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:aaa22383c809c9f23125ef885bffa014040903cf1cf1008872c16a81de943b5f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4570718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac63f03657f633c1b7e4dcfa469f560c160b8b8ac5b71c6267553ebe540bcf6f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:6296ecd945f28c85cb61e65774905755f428d9328193daa24ce25405462ec4f5 in /nats-server 
# Thu, 28 Oct 2021 22:19:59 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:19:59 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:19:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:20:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8049c114269c05bea67059536f0aeb734f038ee927483d627e34e3e2c4c0b18e`  
		Last Modified: Thu, 28 Oct 2021 22:20:49 GMT  
		Size: 4.6 MB (4570243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a45b7c4c5b68b9c73cf5b20d136e7dfe0211c9c4f9c58a4e8a16d6cac2036ed`  
		Last Modified: Thu, 28 Oct 2021 22:20:48 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:74fdc1a3f6e84926d7dc8110da6b901e968eaf257e5cbdb327aa7dbd930507de
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4232588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf98bb7290367ad18d69f3fd515ec2998da6d7ffce6d7e60db06001800aed9fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:57cb553f627f367de9a84332e10da09ed35461fcb69637c3c10c02dd7f98bd42 in /nats-server 
# Thu, 28 Oct 2021 23:06:14 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 23:06:15 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 23:06:15 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 23:06:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:157075e28b5a314b3545fb6763e0276e65c40a7f3d5eebb94cd72ac811ed178e`  
		Last Modified: Thu, 28 Oct 2021 23:08:35 GMT  
		Size: 4.2 MB (4232112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec01e5cb0f5cee3cc803922574720a68bccc229445f64f85bc1229d0785beffc`  
		Last Modified: Thu, 28 Oct 2021 23:08:33 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:e56857df027015a971c4a9dd789dacb54f3b1fbc75e9d71ccf5cfaa4aa8f0acb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4224577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd65fa89f27d041e77778c52c55e94c01ef65de7164a5f7870c9878977043c91`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 29 Oct 2021 01:09:10 GMT
COPY file:ac0bfbbd5aa21448ba6535985198f43830432396e73585d3f489f311676f5b70 in /nats-server 
# Fri, 29 Oct 2021 01:09:10 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 29 Oct 2021 01:09:11 GMT
EXPOSE 4222 6222 8222
# Fri, 29 Oct 2021 01:09:11 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 29 Oct 2021 01:09:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:38f05caf90a106da576ffeaaaab559291547bc712dcea53d610043a3519311da`  
		Last Modified: Fri, 29 Oct 2021 01:11:37 GMT  
		Size: 4.2 MB (4224100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b53084bffe9c69623312340748e7d20197bdfa8b2e07755df383ecc36c8a77a`  
		Last Modified: Fri, 29 Oct 2021 01:11:34 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:77d5afbee4abb94c46579779b4ea4e93a548ebc07c6fbc6343b124f7e3e17634
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4179207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0200ed77c99c0c9b7271b498af9d3181924ce7dbce4ca2be50d86334b479a869`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 28 Oct 2021 22:43:54 GMT
COPY file:7d88722636cdc2ec8d64b20fa29c701d553101eea1d86d44fea56746bd35d60e in /nats-server 
# Thu, 28 Oct 2021 22:43:55 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 28 Oct 2021 22:43:55 GMT
EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:43:56 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 28 Oct 2021 22:43:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9f48f6ea2e66fc81e121edb0d7c05d9ebf5189d2c12bc495305b35aef0dca8b0`  
		Last Modified: Thu, 28 Oct 2021 22:45:08 GMT  
		Size: 4.2 MB (4178730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a086df7f8fcd4b8969befbe3183f0e93ab60633d369f142bdf3f428bc0125b4`  
		Last Modified: Thu, 28 Oct 2021 22:45:07 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:d0f51631445a909756718369391aea239a5e66047cc8c1e23f27116b38dec1d0
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107292363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fca59f0ad00040ce2fd53f9064b408104a6b2683a565ffe6f93cf30b6a02e250`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 28 Oct 2021 22:17:34 GMT
RUN cmd /S /C #(nop) COPY file:da1c8e19512b4f5ec4aafee8ff5f26d969adaa4bfd1d50fd0fb61e3fee70b965 in C:\nats-server.exe 
# Thu, 28 Oct 2021 22:17:35 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Thu, 28 Oct 2021 22:17:36 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 28 Oct 2021 22:17:37 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 28 Oct 2021 22:17:38 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74877abdf9663554ab79db643aab44fcae7a2997c3df7484a1307381e3642ff8`  
		Last Modified: Thu, 28 Oct 2021 22:21:14 GMT  
		Size: 4.6 MB (4624673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80a8a285f6ee8a112f28d907b43e32e3a5013fae158cf167efc21969f10fec31`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a802d473a2f40598eda6d7e288e4ab3f095891656c69668d7caac5a60145a346`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6547e9ec2af9042d8387a4da3ffbc41ed25e6030b0a4433fa0795293ca15d2fe`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab4b6aa5305d791783bbf0e6883f218b27d6a10cfc830a13a09f9b3117544629`  
		Last Modified: Thu, 28 Oct 2021 22:21:12 GMT  
		Size: 1.1 KB (1104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
