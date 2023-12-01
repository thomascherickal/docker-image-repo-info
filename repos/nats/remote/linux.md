## `nats:linux`

```console
$ docker pull nats@sha256:f3248d64af0e7adcbcb21f2c1b3b535152b24a57651c6a4b600c7d359401e6fb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:13c8d74fcc1a65baf6183ffd2fb0e6bf203c1733604bce5ed976f92899c4908a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5482912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c915a3a784500564d97666dfd079f51bd760ec9381c8e37672164ee5a8814dd`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 09 Nov 2023 23:20:15 GMT
COPY file:eb240b5bffcc0f613e659042b381fda542cd7e880986c213f55614d8c9cd276c in /nats-server 
# Thu, 09 Nov 2023 23:20:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 09 Nov 2023 23:20:16 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Nov 2023 23:20:16 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Nov 2023 23:20:16 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cba24f033da718f2444230f64e704439d7f2b84fabfc969c8d76bb9384846971`  
		Last Modified: Thu, 09 Nov 2023 23:21:11 GMT  
		Size: 5.5 MB (5482403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e73b7f3a0e802d16548b50a27050fdfbbeeceab3baa40b4d8edcd30ce2e9e4`  
		Last Modified: Thu, 09 Nov 2023 23:21:10 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:421d1767385b08776c07cf944e3e2773ed237e7c88475daccc534a3724db82fe
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9775bb881f443e9fa40d5e9a1d490d6c0ac2285884e6ef1db0587ea44cc7f89c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:47aab0a4e079835219d1030ac57b665520ec3b3556b447dc66136bb89ed51620 in /nats-server 
# Fri, 01 Dec 2023 21:49:38 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:49:39 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:49:39 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:49:39 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6e8f8b61d8976a4c578b969c4a4359423303568cd8453dcd3e6267ea6f9c780`  
		Last Modified: Fri, 01 Dec 2023 21:50:24 GMT  
		Size: 5.2 MB (5204590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba7048cc7053c12b18a4e6a10a5abdb7eefb2ab0232e8df857e2c9bcfe76b5a`  
		Last Modified: Fri, 01 Dec 2023 21:50:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:4e27083984b59f53b05e3d3fe2c329ead02e8da1de51d8b5b5e36f0163e51eeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33e61a93c2bcd69dd3cc0056fa3dcced16151d82fe5894ca67d431401b846fa3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:0691438ab41edb0248cf73ed7d0b1ce90e953bbf8489017bf463fe9f117a869a in /nats-server 
# Fri, 01 Dec 2023 21:57:57 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:57:57 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:57:57 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:57:57 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f42f5c405f3c6af4aaa299f2260f7a75384153608090bf2ae356b17535387ae5`  
		Last Modified: Fri, 01 Dec 2023 21:58:39 GMT  
		Size: 5.2 MB (5195325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f254d562fb4ca566aad60741716e0d0bba9845349425dfea6cb53322cb6f337e`  
		Last Modified: Fri, 01 Dec 2023 21:58:38 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:fc49857e5161bb3e3dad8c4e450196ef6240679046f2f8ae3d4ad1555b53b462
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.1 MB (5060133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bf654d4be4cbb5cffb66330ae316b3502f5a4b0583ac92d155992725368b512`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:cd59c138ece3c0861debe501271e926bfef17422ef224fd97ff8521666f8b098 in /nats-server 
# Fri, 01 Dec 2023 21:40:30 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 01 Dec 2023 21:40:30 GMT
EXPOSE 4222 6222 8222
# Fri, 01 Dec 2023 21:40:30 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 01 Dec 2023 21:40:30 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1a6d117ef340762e7925ed814b96c617039656b1f96892e5bb171c715f0dd4c1`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 5.1 MB (5059625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74b366db72f5b293b026319031fa62562bc84c616d73a69e19ed161629978949`  
		Last Modified: Fri, 01 Dec 2023 21:41:12 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
