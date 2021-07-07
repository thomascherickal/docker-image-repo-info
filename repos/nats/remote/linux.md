## `nats:linux`

```console
$ docker pull nats@sha256:f84c27c3d970b6726225cd7593d7726046d6026cccc8029049ddb62f6e12cb41
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:da01747b3b1b793d26f23d641b1e96439c8a4a7e06f996382ad5a588b3f22e9a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4338624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72641b68d54bc7007ad321eb3eab0f114b2744342ca010c87f647f84c0b86bf5`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 07 Jul 2021 00:20:42 GMT
COPY file:697b18ad11c92732a089bd820afbe690cc8392744bc144a4dd94fd2d25aba511 in /nats-server 
# Wed, 07 Jul 2021 00:20:42 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 07 Jul 2021 00:20:42 GMT
EXPOSE 4222 6222 8222
# Wed, 07 Jul 2021 00:20:43 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 07 Jul 2021 00:20:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:411fd8300ee124a1c5d0cc25aaede18c5e3b9fcf63ad8db3e23a2a589145d0a0`  
		Last Modified: Wed, 07 Jul 2021 00:21:35 GMT  
		Size: 4.3 MB (4338149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7214f5e8798288f091409c5b65e7d796a10e7924cb3aab9f85ea83d1837dca61`  
		Last Modified: Wed, 07 Jul 2021 00:21:34 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:10e7a6e6d867ebd758bf904af84b0b725fe3881e70046ff67264b5704af885a7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3996729 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f53845fdcc1848648c95df6d5bd3f8fa1853a208cef732a75fe9a11ed645b30a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:9b9474b3d82fa3717ebe79ba7a04cb848a8eaf3253d4c8f3766791d6b7f68a78 in /nats-server 
# Tue, 29 Jun 2021 23:27:01 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:27:02 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:27:02 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:27:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:be0f0fff043a382a22c02d6f84cbd711427028711a5fbe533f14725f6d0e26c5`  
		Last Modified: Tue, 29 Jun 2021 23:29:21 GMT  
		Size: 4.0 MB (3996254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b313a28430c439377c6cc8b91efad91ff87a77989d18f248bdf879edd09e8b9`  
		Last Modified: Tue, 29 Jun 2021 23:29:19 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:16ec0485f0134f1b2726b941699ef0bae2d518ed9cd1f8c54a5c25de362c7048
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3992261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90eebcaa7e2a5fe47f777ab7511b19ac5b27cd487acca77b60a60eede3fcceeb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:fba98ec5a80e29c63bf1f791dc56fc74c146b48e8bde470bbfec822ff9327c38 in /nats-server 
# Wed, 30 Jun 2021 04:58:18 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Wed, 30 Jun 2021 04:58:19 GMT
EXPOSE 4222 6222 8222
# Wed, 30 Jun 2021 04:58:19 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 30 Jun 2021 04:58:20 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ae2295bb426b2954a1fffeae1b800f0be8a8a2fbb7f4421359f312c9bcc8df1b`  
		Last Modified: Wed, 30 Jun 2021 05:00:40 GMT  
		Size: 4.0 MB (3991784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5db3e66f101974822438c934e9ecb9b7ceae76b67cc77a75f4bdf00383283e4`  
		Last Modified: Wed, 30 Jun 2021 05:00:37 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:592123d5f20050bdabd6a76dce8a2c20d5513506cc5e9e42d838bfdbfabcd3b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.0 MB (3960170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebc858fcc364824e208b06d14f783f5098113f0e63b5b50da8598e222f872f10`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:34831d32d44ab42e0d1db98d557ef7f0c98ec4324d06dc1c65d28a9bc4445565 in /nats-server 
# Tue, 29 Jun 2021 23:29:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Tue, 29 Jun 2021 23:29:17 GMT
EXPOSE 4222 6222 8222
# Tue, 29 Jun 2021 23:29:17 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 29 Jun 2021 23:29:17 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d652a8e167e686abe1b85f9b019cf11a7b1696cd8222748e9abee4fd74be6769`  
		Last Modified: Tue, 29 Jun 2021 23:30:40 GMT  
		Size: 4.0 MB (3959694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b01e030a401fa2f5f03cc5e1c6f540631fc77fd52ffd1ef973f2b07dce2ed9ef`  
		Last Modified: Tue, 29 Jun 2021 23:30:39 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
