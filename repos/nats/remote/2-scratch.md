## `nats:2-scratch`

```console
$ docker pull nats@sha256:4fe2c16e211795858e7e7538197ec57f67ed6e9ca5d91d06d925e09ec6724d3b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-scratch` - linux; amd64

```console
$ docker pull nats@sha256:5fd249efa75cf3eb595342175207fdbb390eee3034f7fe49355d7a479fa3ffe2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4499407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c84de17b17b3458d2b6e6d4264ea6186c82bab718ca058f5d7738e53ca2759ac`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:8a814b0c66a47e63e5a7f4287478948812fe6e03c224d539f37ce3f950d2b6c6 in /nats-server 
# Fri, 25 Feb 2022 02:21:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:21:14 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:21:14 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:21:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:277fae1baf41821774f7a2e1c3f465b28aa8693ee0cd77e0ad0bace55d9c616e`  
		Last Modified: Fri, 25 Feb 2022 02:22:04 GMT  
		Size: 4.5 MB (4498900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb932b4b3fbc873b56e996c6357055bb7700c701d17d7d87cdec31211142b49a`  
		Last Modified: Fri, 25 Feb 2022 02:22:03 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v6

```console
$ docker pull nats@sha256:2e3339e7e8d98e7bbab0613c7b7c3dd6f51fcf33ed3910a2e65e62fba7049337
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4165977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ddc7bcc78dd550ace4def82e3db227e618d77e136274749f3bf55869e64be264`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:3a951d885f7bcec693f6fbf26a9ffd82b0c6218b6834fc6053e5812f7451b63e in /nats-server 
# Fri, 25 Feb 2022 02:50:06 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 02:50:07 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:50:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 02:50:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:f6de87b4530f922b11edc08be8edeebc6ce0cb666907013348d4e1b9f5d51809`  
		Last Modified: Fri, 25 Feb 2022 02:52:29 GMT  
		Size: 4.2 MB (4165468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5fa68b52226484e5870677184cdc47c93a7d453f334c144b5cb631346bc8111`  
		Last Modified: Fri, 25 Feb 2022 02:52:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-scratch` - linux; arm variant v7

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

### `nats:2-scratch` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:e970861a260709ae1e8c892eb36758c14323e81959ff4aaa1e9b7327b91d3e70
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.1 MB (4143805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e4414e48026697a15338f28dcb8e46ace9627ea7332559e1708f36ce62a5e327`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 25 Feb 2022 03:01:42 GMT
COPY file:acd11e9a3a86f6f3da079c5155851337e747c3b31481ec05e2dd1e48e23becb2 in /nats-server 
# Fri, 25 Feb 2022 03:01:43 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Fri, 25 Feb 2022 03:01:43 GMT
EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 03:01:44 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 25 Feb 2022 03:01:45 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6ad9fd47af885b43442590ad2c8171e4b4899caef84921ec73ba0540b9c03284`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 4.1 MB (4143299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02d7667f81936503f26a5ed657cfffdc9add626da8ae5bb78d691054cd3af7c3`  
		Last Modified: Fri, 25 Feb 2022 03:02:59 GMT  
		Size: 506.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
