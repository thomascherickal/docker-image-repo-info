## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:16122e63a754b675121e8f119b76fa442df0a4ce9d559a7ca753d0f226e322a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:738d7e11d4e060e168502999f96e4484e53b69f19f3badabe0b6849ba458752f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **7.3 MB (7280037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6770bd180dcf6d53ae5677624eca3e0ab915e0534d7a8ebfb0e23dabf23c09`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 15 Oct 2021 23:32:46 GMT
COPY file:51c48fb54a6e56477646808d811e50530e6cc73cc06456afbf92c93315c7adb4 in /nats-streaming-server 
# Fri, 15 Oct 2021 23:32:47 GMT
EXPOSE 4222 8222
# Fri, 15 Oct 2021 23:32:47 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Fri, 15 Oct 2021 23:32:47 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b5672f16c33de3b309aed8588c76dacfe8b333af776d179a6143eaca2a9311f5`  
		Last Modified: Fri, 15 Oct 2021 23:33:30 GMT  
		Size: 7.3 MB (7280037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:a0c56492ffa63a55221269e1faeddce8417dc9ff787ebfcb86a65af56b28ab17
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.8 MB (6758559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a704bd4cbe4a263f4ebc18672d20e48522bfec086637708c31311855f6936402`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:10:15 GMT
COPY file:a76fac69ee7921326b516d57954b5c72bad76e046253d3ec9da3fddebb4c2001 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:10:15 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:10:16 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:10:16 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:785631e7402301196781d109f30a49ca1e1bb7fc10fbc4aa5502d3c42fa0bed4`  
		Last Modified: Sat, 16 Oct 2021 00:12:10 GMT  
		Size: 6.8 MB (6758559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:a5e3d56b343f9091f353634f59f688998544ccd4f2cbb80001d08ea6a3207274
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.6 MB (6639768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80206ae32558812ad047d8ab67519615e98e7df68a884fc32b6d5fd8f72593b0`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Aug 2021 23:11:17 GMT
COPY file:79708b5d249193a95e72c506453fd1ecd3e2738ec2ff3423c4b2bd760f426da2 in /nats-streaming-server 
# Mon, 02 Aug 2021 23:11:18 GMT
EXPOSE 4222 8222
# Mon, 02 Aug 2021 23:11:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Aug 2021 23:11:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:52753762f751e166edd44e37a0ef0a06b33c337bdeb66e4134ee8479a49dae68`  
		Last Modified: Mon, 02 Aug 2021 23:13:17 GMT  
		Size: 6.6 MB (6639768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:73613ef7449fc409f5bb72b2c43fc67f3541cbebdd2ce877e3bee3f1c2d452b2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.7 MB (6651802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fecdbb78af38acba0e12830aa8daa69ed2079616ec837b357987762c85470b6c`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Sat, 16 Oct 2021 00:03:17 GMT
COPY file:e0f0edd281288af78ab5d195a8de40dfe0253996c368426c7085ec08ea8a43f0 in /nats-streaming-server 
# Sat, 16 Oct 2021 00:03:17 GMT
EXPOSE 4222 8222
# Sat, 16 Oct 2021 00:03:18 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Sat, 16 Oct 2021 00:03:19 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:6c0a26bcc42887a4b359ea4c856e11ba7fadf97bda213d9f09da276e5bfd0abf`  
		Last Modified: Sat, 16 Oct 2021 00:04:20 GMT  
		Size: 6.7 MB (6651802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
