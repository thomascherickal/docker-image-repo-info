## `nats:latest`

```console
$ docker pull nats@sha256:4fa6d62e36bac738598e6523bb2185b0d57de021331057a538765f518cfd505a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2565; amd64

### `nats:latest` - linux; amd64

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

### `nats:latest` - linux; arm variant v6

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

### `nats:latest` - linux; arm variant v7

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

### `nats:latest` - linux; arm64 variant v8

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

### `nats:latest` - windows version 10.0.17763.2565; amd64

```console
$ docker pull nats@sha256:d7c795020fd7295382d503ba883e23cf34ca9c53d6e6b91184bc1fd2bb2c990d
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.6 MB (107634881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e99776e94a148ebda875656d07e673c65aedb583986faedb3bdc61a2fd7759`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 18:13:36 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 25 Feb 2022 02:17:30 GMT
RUN cmd /S /C #(nop) COPY file:d5609a37f534b519fa4326428362ea5398f7165ee90493fb7bdc8b810da33b0e in C:\nats-server.exe 
# Fri, 25 Feb 2022 02:17:31 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Fri, 25 Feb 2022 02:17:32 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 25 Feb 2022 02:17:33 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 25 Feb 2022 02:17:34 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8bc49c59cde14e3a9ed8fedce001c00fcb5fe0f9b914aa07273e04f23333d180`  
		Last Modified: Wed, 09 Feb 2022 18:14:28 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b682f8d539489225b7a3859570b80452b497086f57fa4e6908f2b99d213e1a03`  
		Last Modified: Fri, 25 Feb 2022 03:15:32 GMT  
		Size: 4.5 MB (4541735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67997158a056ea601aec06de195ce0251264a6d8d071f8a44a49a545865ce426`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.7 KB (1656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f873036aacce9bbc35378d6a36985e62919c6d2c9ff526011564a861b86240ab`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.0 KB (1039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1eace4b7f44dce795499001f62baee27fb477865e490b11d05d198c8e80550`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8accc8a69e6317ee43a53e093f2aef25b70ddff625cfa691d7df28e9bf6d94dc`  
		Last Modified: Fri, 25 Feb 2022 03:15:27 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
