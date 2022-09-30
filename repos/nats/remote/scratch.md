## `nats:scratch`

```console
$ docker pull nats@sha256:78fb2aa1056a6d74fbaa7b0c636f75751c2957227a5b69543e10063ed74f8de2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:73a511425369d8e883fc5784023028b7ed02c252e6db030e776b2e6a76bb90ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4907513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf3ba31eb02c938f2ab28c2b60358ef903503ce4a2fb5e2df6f4714d04e74619`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:ef7d265008705c7f8da964d29a2883d21303aab4d4520c3327ca6ce57348e137 in /nats-server 
# Fri, 30 Sep 2022 00:25:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:25:01 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:25:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:25:01 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:25:01 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:325d5a714be1f0303eebb8d34c9b23e1b15c5e7e46eb29d0f90511112fb86894`  
		Last Modified: Fri, 30 Sep 2022 00:25:50 GMT  
		Size: 4.9 MB (4907005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b03a363308e84c4fc60d5ac2d5b9374e811456edecdb1e302e59198bfb1ca4`  
		Last Modified: Fri, 30 Sep 2022 00:25:49 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:22be654fd606d7db5e28383ce35794c881f25b77908c6f981c2442b117d7df19
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4671534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eeeee00c7520737eb3766018dde7f3dd63c971938d98ff49cca225f0e6c6990`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2de52eed8721a4ef1e4c8adb2f046a7ffa8e689d614c704b329ef2bafc7dfe5c in /nats-server 
# Fri, 30 Sep 2022 00:15:17 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 30 Sep 2022 00:15:17 GMT
EXPOSE 4222 6222 8222
# Fri, 30 Sep 2022 00:15:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Fri, 30 Sep 2022 00:15:18 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 30 Sep 2022 00:15:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:948e55d9b8c745ce1f9007c64a6da65d66c0d554fa7e5808a04081a1d0754a6c`  
		Last Modified: Fri, 30 Sep 2022 00:16:49 GMT  
		Size: 4.7 MB (4671025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14bdee3fcf17688810034aff56b746397e799579ff11654f2a2ec59274a9e161`  
		Last Modified: Fri, 30 Sep 2022 00:16:48 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:03a39590b94ba73f75c39970947a3ff276c7f37d7e6e8009ccf780251f6cbc81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4660097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f35ae12fca7c133fb2e99616ac3d87777680804b3654472e9c4d78d28db4e965`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 22 Sep 2022 23:58:10 GMT
COPY file:8333f5a10c97b92118357725370604074ebcfef54b0d6e7d818b8a5280ac8fee in /nats-server 
# Thu, 22 Sep 2022 23:58:10 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 22 Sep 2022 23:58:10 GMT
EXPOSE 4222 6222 8222
# Thu, 22 Sep 2022 23:58:10 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 22 Sep 2022 23:58:11 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 22 Sep 2022 23:58:11 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:131d7d99719c2d3afa300226a95a811f986eb26f05d0aa3bd08fda92824f90a7`  
		Last Modified: Thu, 22 Sep 2022 23:59:35 GMT  
		Size: 4.7 MB (4659588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40b4198acf76381af038bfd14e9332c1ccd3a7235889f327c2d387fbd44b1b3`  
		Last Modified: Thu, 22 Sep 2022 23:59:34 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:080acc4ece31f7fc871e35471f286e4991b8febfe1379f1fb6b1e0d6eac551ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4494416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5d3fd2d5a277619c0411f028a92dd0e001aaf241be51e3bfc66db595c651f32`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 22 Sep 2022 23:40:22 GMT
COPY file:78383a44c18e587e522cc9799431581c891b0ef3afdf06dee4c7f7267ca8bde9 in /nats-server 
# Thu, 22 Sep 2022 23:40:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 22 Sep 2022 23:40:23 GMT
EXPOSE 4222 6222 8222
# Thu, 22 Sep 2022 23:40:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 22 Sep 2022 23:40:25 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 22 Sep 2022 23:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3708e85fb8eb51ba8efd3211608a7049a9714a9f0f6282c1d78fb3efc99abed8`  
		Last Modified: Thu, 22 Sep 2022 23:41:42 GMT  
		Size: 4.5 MB (4493908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee57fd3c887f07b3980dd16bfc149abfd66ce3cba86f7e877dfa055492cba071`  
		Last Modified: Thu, 22 Sep 2022 23:41:42 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
