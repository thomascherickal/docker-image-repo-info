## `nats:2-linux`

```console
$ docker pull nats@sha256:2f9e57c99ea73b5104afac918473211db5ddcd1a6b4434350c84ff56b623827e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:b320fcb71942b77a78f93bd3989db775fed560bb338289167f1cf75323ab6d64
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4480339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4469d7e4ed97c5ae7e12c6d59a9abc6e33af6310fea0bb9a762d4658e6cf2c36`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:20:28 GMT
COPY file:118dd4676051de91f454ec7318766cc4df73da9312c0e1729b5f38bc804005dd in /nats-server 
# Wed, 26 Jan 2022 01:20:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:20:29 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:20:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:20:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0822339f45b3d6ed05ef647342264f4451e612fc8bb64d82964896e365828856`  
		Last Modified: Wed, 26 Jan 2022 01:21:22 GMT  
		Size: 4.5 MB (4479830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9be98f352bc7c2a94dfae4fdb49aed3960da13d7cfb5018ee21739dbf8fd22`  
		Last Modified: Wed, 26 Jan 2022 01:21:21 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:9afcdc7c11f71cda2dc7455df3e4652f400e09f521105355698bcf5aad9ef803
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4144655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9bcf5d7dff9299abfb6707c4b41e610b7f1d3ecdf606461ca559ca7660d330c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:50:05 GMT
COPY file:b2ecfebbb565fc6384df7e48dac9ce60eef17b2f48a3b3a2f48a1ab3664f2639 in /nats-server 
# Wed, 26 Jan 2022 00:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:50:06 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fdf2fda9877ccd8e5bec73cc0c3551520bef9ef875fda99ca166b6a2ef01cae8`  
		Last Modified: Wed, 26 Jan 2022 00:52:32 GMT  
		Size: 4.1 MB (4144146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32f83944f51f08946a79783101063c668ddc63777a0803280415734fc8e0e2e`  
		Last Modified: Wed, 26 Jan 2022 00:52:30 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:fa219cbe43942f4113ee518cc0a527cdde5d7311b78888f005f4d28137c98b65
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4138057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef43179a4ad3fff1073403697dcc92ce785caf5df9353b17b118ef5b34dfdbb`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 00:58:25 GMT
COPY file:5f30a1a4bcfa1627334eb39b98e476082bfcefc1ed0163a244d31f6055f14986 in /nats-server 
# Wed, 26 Jan 2022 00:58:26 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 00:58:26 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 00:58:27 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 00:58:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a857ca3b7114803e9d91321fecf0baa61fd0bf4bf10bf7b5f0cacc3d75a85189`  
		Last Modified: Wed, 26 Jan 2022 01:00:53 GMT  
		Size: 4.1 MB (4137548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a37b83ea007f8d2f717c783ee4db28e103db7c16c334230afc85dbf5088e7d4`  
		Last Modified: Wed, 26 Jan 2022 01:00:50 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:a0948ed6fa514188f09cc7748f6485a8de368a392d82a774dc1770082f4a7526
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4125231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d5f9ba9462775ca2785ed2763f505fdab174798c869a1cdec6b4d4935f5ba54`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 26 Jan 2022 01:55:38 GMT
COPY file:d68e1ff180064a09f016e0ca24ee1a156a781fea15000819ce03a38048a74fb2 in /nats-server 
# Wed, 26 Jan 2022 01:55:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 26 Jan 2022 01:55:39 GMT
EXPOSE 4222 6222 8222
# Wed, 26 Jan 2022 01:55:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 26 Jan 2022 01:55:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d67651f2d8c13fdfb8ede24c731d7d43f311448e7334044ce929aa1a0879788a`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 4.1 MB (4124722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b510068b87eadba39d66536bfbdc4942364be73dbdb1c1a51108f3110368e3`  
		Last Modified: Wed, 26 Jan 2022 01:56:56 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
