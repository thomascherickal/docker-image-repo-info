## `nats:2-nanoserver-1809`

```console
$ docker pull nats@sha256:f39d40887447d130084e58b0e3d24c7eea3d5282c503f668f5eddfb6105151e5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:2-nanoserver-1809` - windows version 10.0.17763.2237; amd64

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
