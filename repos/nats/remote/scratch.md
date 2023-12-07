## `nats:scratch`

```console
$ docker pull nats@sha256:2157b210fa06c7fdb1cc8f9f27accf1b75165cba57eacd05f5ce29b33a12cabd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:3976691a844ea7e9dd27c2999792b60e03425063cf929cac8e2124de06ed3560
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5487590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c26f92862c0582fc993931f218754dad07ee673b6546207c14c567d225b6e63a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 02:39:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:b293dcd5520198b4ebacbb23e1a20b58933a547a716641a4a49593689943c555 in /nats-server 
# Thu, 07 Dec 2023 01:20:04 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 01:20:05 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 01:20:05 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 01:20:05 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:55b7ce72608a47e5a7bd1e39940d1bf067c5a618509a681e424dec3f41ad193e`  
		Last Modified: Thu, 07 Dec 2023 01:20:52 GMT  
		Size: 5.5 MB (5487082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47726e1b8bcbdecc0b802542585b4fa0292d250b3510f7bea52a37b7770829f`  
		Last Modified: Thu, 07 Dec 2023 01:20:51 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:25e7841f5b4c74faa1cefa3ac3a9b676cde24301bb4457381d45a631aeaed3af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5205300 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0df98ee98ab731da5630054247a95f41befffd2873016036e7fe10c0f93ddb4`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:29:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:57db66e8f632416070a8742db1e78e42b6a00178d3cafbb1d951f712bc1528b0 in /nats-server 
# Thu, 07 Dec 2023 00:49:31 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:49:31 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:49:31 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:49:32 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:dd9254a38d172bab9b5d4a85c3955a5bf8dc94569fdf541322f3006b8087cec0`  
		Last Modified: Thu, 07 Dec 2023 00:50:20 GMT  
		Size: 5.2 MB (5204791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30653da0be2fe0acec3ba9ba2b603cc6aa9511b5d611c70c10ecdd9b0709ad51`  
		Last Modified: Thu, 07 Dec 2023 00:50:19 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:2f076475563abd22dcf74c6af677e35859ccab3a754d5a281658c0d9d5c2616b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.2 MB (5195996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30c5b8e257b98246d38116c31cbe591849717b8ab84532e3a015a86266685b85`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 21 Oct 2023 00:53:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:482f302fa9d7fbd341528e0f1e03e3282081407a2d386be43ab383f493ece9b9 in /nats-server 
# Thu, 07 Dec 2023 00:57:52 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 07 Dec 2023 00:57:52 GMT
EXPOSE 4222 6222 8222
# Thu, 07 Dec 2023 00:57:53 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 07 Dec 2023 00:57:53 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:97255bc6d162eeb7b3d0263f62734c0ef45732bc93eb0063e914122f0eb6765a`  
		Last Modified: Thu, 07 Dec 2023 00:58:37 GMT  
		Size: 5.2 MB (5195487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc1a79f36d37d186ce94726a14aa24c287066ce1bf5b22c3f175bb80c42e07f`  
		Last Modified: Thu, 07 Dec 2023 00:58:36 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

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
