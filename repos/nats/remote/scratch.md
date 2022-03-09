## `nats:scratch`

```console
$ docker pull nats@sha256:c5138097a7d91355c8ea3cb82b11f0bcdabae08a57191b7e0249b4322240385a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:scratch` - linux; amd64

```console
$ docker pull nats@sha256:5102d9ad6d58bc95c08d14e8fe54b4cb432ac9237cec01d33dcbd8e4850cf447
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4510590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7d053ccf4f981153bfbc620038e1ef8f4350bd08832ada50fb0a0fba84572be`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 22:25:51 GMT
COPY file:02a472480673a11c995d1ea52b63c55910490337313c1211b4877f5071117f27 in /nats-server 
# Wed, 09 Mar 2022 22:25:51 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 22:25:51 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:25:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 22:25:51 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 22:25:51 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:d9292be658bded2e584005b2d2d3c989d58b8c84c43d30cbf498884e4da11d88`  
		Last Modified: Wed, 09 Mar 2022 22:26:40 GMT  
		Size: 4.5 MB (4510082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c053a12f02cf2d3d90a7d26739c64349d29833ccb5f6d04c6b28d8fff2443538`  
		Last Modified: Wed, 09 Mar 2022 22:26:40 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:3256353a8d53c6257a1ec8c17b572529f87360bf3b105b470da8998266e05315
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4174562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5335fe9c64c80865dd34d7f1d94b52b6d4038ce714fb04d9f318a0393262dac7`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 23:06:00 GMT
COPY file:63d2dc292853c2a6d99433d1e8a92c091a0c775ab65a2e453be73d5448e05594 in /nats-server 
# Wed, 09 Mar 2022 23:06:01 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 23:06:01 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 23:06:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 23:06:02 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 23:06:03 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1c9142de49642e016c3df123dce55998ce71f3777b9433742a88aa91b23f9ae9`  
		Last Modified: Wed, 09 Mar 2022 23:08:21 GMT  
		Size: 4.2 MB (4174056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232eee2ffad4b2ab84d1a4aafd3be0df1c1066f57eab6f18a4b55344b74488be`  
		Last Modified: Wed, 09 Mar 2022 23:08:18 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm variant v7

```console
$ docker pull nats@sha256:87cf3f8e33ebf28f35575ea083f8feb460d19fa9380d2622c82567ff3fa9d840
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4157918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4eef99b95e572b23f90d60e6e157be90b05ab2f35dbcb10f83f96ece551945a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:3ee879939ad264e803dd4d6072181d968c4dd0fe076115159f70479c6309ef45 in /nats-server 
# Fri, 25 Feb 2022 02:58:34 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:58:35 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:58:35 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:58:36 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:67a3d8907097b9caffd9d1720b4fb2b1d2ac9dfda60a1d169abbf5494323d50a`  
		Last Modified: Fri, 25 Feb 2022 03:00:58 GMT  
		Size: 4.2 MB (4157409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5577f4846f032b281220b897161962481198ead0a1b9ad1d7c76cdd989747`  
		Last Modified: Fri, 25 Feb 2022 03:00:55 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:4cb4ef773edd64ce015945185e30502ff5c80ea967e3ebbdf0f8d3751016ff45
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4154621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67bb252022527ea75cce7f45ea7463fe04e9e5b5628152fb157822c0d01bc139`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 09 Mar 2022 22:57:14 GMT
COPY file:6d6603ade462e58030bc93029992af55dac8b9eae7e4985b5c84dd49e1ee1be2 in /nats-server 
# Wed, 09 Mar 2022 22:57:15 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Wed, 09 Mar 2022 22:57:15 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Mar 2022 22:57:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Wed, 09 Mar 2022 22:57:17 GMT
ENTRYPOINT ["/nats-server"]
# Wed, 09 Mar 2022 22:57:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5663127c1a3d9c378ea8ac20e94b430188a9dbb2675ca0b26205f9a5e1b0bf36`  
		Last Modified: Wed, 09 Mar 2022 22:58:35 GMT  
		Size: 4.2 MB (4154114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bc2c19c0a6d2b137b1891d3ee3716153114e9575e2a1bc966dd0660a4c7b72`  
		Last Modified: Wed, 09 Mar 2022 22:58:34 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
