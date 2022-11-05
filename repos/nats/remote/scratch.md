## `nats:scratch`

```console
$ docker pull nats@sha256:2b8509f09b126afa979768738a2227a0d42105f5febd2f7be5801b1a803fddc7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:e0c120189c1cc4105083260125394f531e00a9baaf11cd0e000da67f20ded151
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4912228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c36450b96e54135d8ae5c240c9b77aea9695e8788641933a984e45ade8eb280`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:ef06448123f717cc9d112f122946b32d23041ca982de308f34f661bffbfd776e in /nats-server 
# Fri, 04 Nov 2022 23:30:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:30:54 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:30:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:30:55 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:30:55 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eb67f80a64092aa558f62b5fe50105f037ad11be30e6e41aaa6edfb4ba13dfba`  
		Last Modified: Fri, 04 Nov 2022 23:31:43 GMT  
		Size: 4.9 MB (4911721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f794b37309be915cd84f81f15ab88748d4a002af66d370bb008e160a66ed22b6`  
		Last Modified: Fri, 04 Nov 2022 23:31:42 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:b7d7f838330af8f53d3bcfd355ab7ae938e994fe6ef1b9c4d715e41da214b9f2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4679036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2ce2b8bb877b0120514a5bfff5733c56fa4c7389de944f1431b0c7aed345bc6`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:297fbf7821eddb0f824a39683247efac5dd7394045d7e57a1c0349162e916362 in /nats-server 
# Fri, 04 Nov 2022 22:49:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:49:43 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:49:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:49:43 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:49:43 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d3f31c0919e9695fadb96f15fcaae47a1a9fc01df15b4438e5107d7f16eb02b6`  
		Last Modified: Fri, 04 Nov 2022 22:51:21 GMT  
		Size: 4.7 MB (4678529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dbe7df02698559d095933c9489404d632e731b7212aa96ee3102925509e25ca`  
		Last Modified: Fri, 04 Nov 2022 22:51:20 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:75575821072dccdfa91a38e833e8f9c050f134bb0ff3a2d2638cf8d8f9e7a4d9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:022e28a8cb84d94c0260db6bd140127b0703b45c38573911e514520b0e7f1fca`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:70be153a513a336de6070d6b06734a08c8d3c111487664d8171d3ad2e560a9fc in /nats-server 
# Fri, 04 Nov 2022 23:08:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 23:08:10 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 23:08:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 23:08:10 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 23:08:10 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0f40a6215ad00f24584ae5c5627357ad231b51072ddc0a9afaa07bd995d77503`  
		Last Modified: Fri, 04 Nov 2022 23:09:48 GMT  
		Size: 4.7 MB (4671418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17727ee9e8010b318dd39df7a5564cb586a44f1cb7b3ccb06afdae6d3c93a5e`  
		Last Modified: Fri, 04 Nov 2022 23:09:47 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:89dabf164ecc437ed321d60703fb97ceeb8f6cca5dc50220a2b56f391b3166e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b58178afb650de0100a4eaa29c6297853bab23c50b6c6bf389a9d289d85c3bd9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:b208c02f06c30ef713b7cfd9032cea05a4edf19bcc1cbded3177694bae93a89f in /nats-server 
# Fri, 04 Nov 2022 22:48:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 04 Nov 2022 22:48:15 GMT
EXPOSE 4222 6222 8222
# Fri, 04 Nov 2022 22:48:15 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 04 Nov 2022 22:48:15 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 04 Nov 2022 22:48:15 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ee7e311fa92f195abf7f350c1ad218c99207204a7f43139bf5e28172e2550939`  
		Last Modified: Fri, 04 Nov 2022 22:49:06 GMT  
		Size: 4.5 MB (4498503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698bbdfd5ab1d577fb5190fbe857b016912cb3562ff6a655017b4d0c6663fbb6`  
		Last Modified: Fri, 04 Nov 2022 22:49:05 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
