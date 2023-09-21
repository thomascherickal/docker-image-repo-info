## `nats:linux`

```console
$ docker pull nats@sha256:279c3e1bc63c82126abafed2b06ae0c23cfe06d526db00f0cd2bf790595b1e53
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:linux` - linux; amd64

```console
$ docker pull nats@sha256:300b8159816cb200b0ddca347e2895e811131e89660b698819d6a04d017b51ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5457759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f5b65974bc0ab52f1a6bd8c018ff5fadadbc976f311db512c19acabce037b94`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:49:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:49:23 GMT
COPY file:8e2a9a3f381167fcc1a95dc7718c10cb67f58a845a3197193a5273c57e28d08d in /nats-server 
# Wed, 20 Sep 2023 00:49:23 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:49:23 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:49:23 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:49:23 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:949cbe9ff3fb07dc0fbd1c6fb6ba4a1c20304c28d574891f79f5d84e05439ec0`  
		Last Modified: Wed, 20 Sep 2023 00:50:22 GMT  
		Size: 5.5 MB (5457252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e49c9fc5d845768deddd7c19342fd407ee4fdc4d110abf53e58444440c552181`  
		Last Modified: Wed, 20 Sep 2023 00:50:21 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:cce3ff90a32531db64bb74852140a156326d487dafbf812da2168f78c0e85388
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5178106 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:111b8fef881498596233d1f7dda3dc1a4113c72bfe5e1088ded56d10a45d128f`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:49:28 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:dbe6aeea160dba3a7bdcaf0c14808f7a7b31899bb87a50ed117996ead07014e6 in /nats-server 
# Thu, 21 Sep 2023 00:07:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 00:07:58 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 00:07:59 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 00:07:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6837114cbc023e4b8b17b6a951b2e91ab9668a1f3ffe65bec26f4ea44b812845`  
		Last Modified: Thu, 21 Sep 2023 00:08:53 GMT  
		Size: 5.2 MB (5177597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bde9589f631b3debf2ce00b1154c597464aeb530aac8a0016d7bee37f972958`  
		Last Modified: Thu, 21 Sep 2023 00:08:51 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:41b2a21a345689e5edc4cb8d24444c46df161e58ca89578e66a66e2e0aee2a47
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5171757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed343d1334d5c6f933acaae9f280c90acde044ea41eb6047dc9126ecd17dbd37`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 20 Sep 2023 00:39:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 20 Sep 2023 00:39:39 GMT
COPY file:1ed1e6185c40930f2dc5e0e072cf3d42764ec8f3c10b2f65c3044c6aaf6d5ac5 in /nats-server 
# Wed, 20 Sep 2023 00:39:39 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 20 Sep 2023 00:39:39 GMT
EXPOSE 4222 6222 8222
# Wed, 20 Sep 2023 00:39:40 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 20 Sep 2023 00:39:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9af7ee06c60cdf35e2e953e1ad5700cf513329b5f88bb07096c8439fbdd7cfb4`  
		Last Modified: Wed, 20 Sep 2023 00:40:42 GMT  
		Size: 5.2 MB (5171248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5795401da82ad77eec35f59034d9f5ce5ff6af93cc82c2a00277bf954ef32c2`  
		Last Modified: Wed, 20 Sep 2023 00:40:41 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e6aea49e5eb407c078286700c1402c6eda155ae11cdd40f8604194f6f70d0dd2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.0 MB (5029479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d109a8655a05cb22d5529db631b1a167bfae974cfc5d047c1ac261888ecd6e8`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 19 Sep 2023 23:42:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:943544393eb61c235711dc43a87ec667d4491be8bcff70eee560d8276bd01b5b in /nats-server 
# Thu, 21 Sep 2023 05:05:18 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 21 Sep 2023 05:05:18 GMT
EXPOSE 4222 6222 8222
# Thu, 21 Sep 2023 05:05:18 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 21 Sep 2023 05:05:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:85892a63e455fd1561bc50ef513a999a9a22152bbab4f029732ea77658da0b37`  
		Last Modified: Thu, 21 Sep 2023 05:06:05 GMT  
		Size: 5.0 MB (5028971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24d6a1649b69be08c681087d8f2f84e750824c24acb44b6d1be0a9a706bb112`  
		Last Modified: Thu, 21 Sep 2023 05:06:04 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
