## `nats:2-scratch`

```console
$ docker pull nats@sha256:6153bba8d67fc88c2e132b35625d5d38e9bd306985ec2ccc2d85dcc9e03f53a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:ce50109292cf290d1f6559a806f7e6f1b202f4d97678700dbb386b1d6c021964
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4574459 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fa4b152b84f6a4cc5da9b870074d5807b7dc42dbf1f922c1ff7e3059d6ec1be`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:f554ccd652a698194b4adc9f60df406473cf580a258d4b425944a529b6b7b718 in /nats-server 
# Fri, 05 Nov 2021 01:41:00 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:00 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:00 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:00 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fe57332791af252fb9335dd0de8a36fe319e51fdde00636db3fee85f1adcb22f`  
		Last Modified: Fri, 05 Nov 2021 01:41:48 GMT  
		Size: 4.6 MB (4573985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc9e783378fba5ac033e418e7db34fb0215aeaa59658adf4924ad46455f261e`  
		Last Modified: Fri, 05 Nov 2021 01:41:47 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:a94f85ec4b90db46b3c8d59ed4c35fa9033482dd0e50679775145fc0f2528b20
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4236770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bee36fb33e6c4d4ec54bcbd1778a2d3a19dcd7706111ffaf4d1711e916f6dea`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:0e12b4e14d681c94ae627c578bd9cc8a3fc9bec59e0062a772ad0933b7947e38 in /nats-server 
# Fri, 05 Nov 2021 01:41:02 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:41:03 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:41:03 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:41:04 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:a273e90687e1ad496ce74eecec787df7511839c5e770850a184f261ed706fc98`  
		Last Modified: Fri, 05 Nov 2021 01:43:23 GMT  
		Size: 4.2 MB (4236294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6825ddc1425c3e1cfde24c7f0c22b2ad39646ecc4d15d72b1d4769687206880`  
		Last Modified: Fri, 05 Nov 2021 01:43:21 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

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

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:d7e28f91b2fc35b9a0ed2eb9a5e16070e4c2d1dff3f18076e465958b997cce01
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4182966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:089ea638210c9c36041b15aac4bf873a36e3b4bdca7b8e25d6c1b4cc9a274094`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 05 Nov 2021 01:25:26 GMT
COPY file:2327a2e0254f808bd88c7e734365e343ac6cf801c454a43bf9035cd435fbf8d0 in /nats-server 
# Fri, 05 Nov 2021 01:25:27 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 05 Nov 2021 01:25:27 GMT
EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:25:28 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 05 Nov 2021 01:25:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:fd5084aec62b3e936e8b267729c530280fe1646e8e9d0e09ef842b74beccff33`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 4.2 MB (4182491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963e399425efdeb20d2700e846b7b3f5c36a5ecef7204cb3fe1476b7b835b2e6`  
		Last Modified: Fri, 05 Nov 2021 01:26:42 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
