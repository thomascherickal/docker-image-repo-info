## `nats:latest`

```console
$ docker pull nats@sha256:5ab674f1921eb219dfda75570b44d18bcc4edf78edb76c9157ae9ac09bd0e595
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
	-	windows version 10.0.17763.5122; amd64

### `nats:latest` - linux; amd64

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

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:ca5325d2a2c84eca8c4f3e3ba96a4fcf6dc91e97e3d3ebd3bae69f7a126c0e62
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5248367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea934ed1a17a93225092fac66c8b617c594ecec00debda4eb753479eeadedab2`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:22:58 GMT
COPY file:c3d82eee52a26292cc80755a2b88f8b80cef5c80fd438c99768cd1c33ca95a9d in /nats-server 
# Wed, 08 Nov 2023 19:22:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:22:59 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:22:59 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:22:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:44811b84801c95891b1ccde13fe7e76a1ffd8795cd2a066ac0630ee836c23c2e`  
		Last Modified: Wed, 08 Nov 2023 19:23:46 GMT  
		Size: 5.2 MB (5247859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8927d64e5da79549425963bee122f44117e41eaa442b01673188effd14c9b236`  
		Last Modified: Wed, 08 Nov 2023 19:23:46 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

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

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:4d3ccb1b790e4433d69872d7ddb8377aac40d6f000a66fa5b2795a62122a4f54
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4984842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2f1a1ecd1b37c66268f966a88d26fa44b35f70909dedab19c60bfd5aca2035e`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:49:29 GMT
COPY file:401de119a9fad5bd89c70f5a4d5c70f110d490ae5ab9aa60a7f963686ab297ee in /nats-server 
# Wed, 08 Nov 2023 19:49:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:49:29 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:49:29 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:49:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f1d2c1b6f013f4386e7235452bc47cebd8001115c3a6504b418ee5b90071492a`  
		Last Modified: Wed, 08 Nov 2023 19:50:14 GMT  
		Size: 5.0 MB (4984334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5fea0f4bcfa87853f77179e249f0a8a09723aeb1c53882e3036fa6250a4ff5`  
		Last Modified: Wed, 08 Nov 2023 19:50:13 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

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

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:c73b24d4fb1ad910ad2f2bdefe0d18bfec11431afb4da9e3cd2be176e4fd49b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (4977978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbfe5b4a001ee28a1308edc00242441032b2afb69148c7ba17f692f75e2c1dba`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:57:47 GMT
COPY file:cd8c3bf2b10d14de1f76a0617be080153909dadcd658bb62cab16d41a650d3de in /nats-server 
# Wed, 08 Nov 2023 19:57:47 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:57:47 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:57:47 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:57:47 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e2a0a8d03803b71ab2e1e3540de965b9430b493bbd15bb2cb1372a7dd564c76d`  
		Last Modified: Wed, 08 Nov 2023 19:58:32 GMT  
		Size: 5.0 MB (4977470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bfe9df0b73b8b228e9331792251ba43d36af5e4e898411b4f9b725bb8928231`  
		Last Modified: Wed, 08 Nov 2023 19:58:31 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

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

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:770e514bf6ca4d8b056bd9d16b7df5f56c45c587ce3c815515051b6588e38325
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4785043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b75bc6347feea13831461567c92c52c13e9085417ef409fb74364cf63105e346`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:14:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 08 Nov 2023 19:40:10 GMT
COPY file:209cf40c58f80a36d8d8c8060f48a598dcf03ae451d8d658f267d02f3ce7bddc in /nats-server 
# Wed, 08 Nov 2023 19:40:11 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 08 Nov 2023 19:40:11 GMT
EXPOSE 4222 6222 8222
# Wed, 08 Nov 2023 19:40:11 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 08 Nov 2023 19:40:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b497fc8beff1c9fb319e3b4b62e22135e8e8d81506ede3ca51365887947a8571`  
		Last Modified: Wed, 08 Nov 2023 19:40:59 GMT  
		Size: 4.8 MB (4784535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbc2e7980e0793ef96d07cc5a7d9418109519d7d6982ba49570b90d02b2932c`  
		Last Modified: Wed, 08 Nov 2023 19:40:59 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.5122; amd64

```console
$ docker pull nats@sha256:8f6397e308a0bb75d9a4e99269657514a0aa8a5d8d59cd0b14aaf98859cfe42d
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.1 MB (110100392 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a214813eb86dbbb2a16ea7ff2add0e2bd94055ce3287eb6b4e9f74c605026a99`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Nov 2023 17:21:05 GMT
RUN Apply image 10.0.17763.5122
# Thu, 16 Nov 2023 05:07:37 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Thu, 16 Nov 2023 05:07:38 GMT
RUN cmd /S /C #(nop) COPY file:dbbf376643d913f572787dfa3a580d012b8bc2c35e2734d995eec070a00ee72a in C:\nats-server.exe 
# Thu, 16 Nov 2023 05:07:39 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Nov 2023 05:07:39 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Thu, 16 Nov 2023 05:07:40 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Nov 2023 05:07:41 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:24e10ec0ecb89022cf68752b9f9196dcf2f423f9589b14401693fb2a1b3de37f`  
		Last Modified: Tue, 14 Nov 2023 22:06:25 GMT  
		Size: 104.5 MB (104497517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6482f23797692e3cc4e6739a9923a136f784b599c3f22a9d2ecb0570cdda33fa`  
		Last Modified: Thu, 16 Nov 2023 05:12:04 GMT  
		Size: 1.0 KB (1038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b496a61e44638d3c8f817536b47873a68bc05ac1399fdcdf61dbd01b683da693`  
		Last Modified: Thu, 16 Nov 2023 05:12:04 GMT  
		Size: 5.6 MB (5597000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04eea5e0db79a0a7cde8431775751ccf6a8c5cdde13f9368308a4ecf177903f1`  
		Last Modified: Thu, 16 Nov 2023 05:12:02 GMT  
		Size: 1.7 KB (1707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad44c7f5cfb0da1faa82600c6008510e494ecb4d0a0a25da38a71391e0fd034`  
		Last Modified: Thu, 16 Nov 2023 05:12:02 GMT  
		Size: 1.0 KB (1030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4959acd19fbc0a60140ae3b7c10f21a6472d528bf6a3552feb4503d870b377`  
		Last Modified: Thu, 16 Nov 2023 05:12:03 GMT  
		Size: 1.1 KB (1064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8527b34ad2c965db90687e02e642bfecea5f059fc3e0efc5986537f3d97a173c`  
		Last Modified: Thu, 16 Nov 2023 05:12:02 GMT  
		Size: 1.0 KB (1036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
