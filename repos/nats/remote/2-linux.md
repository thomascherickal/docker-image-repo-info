## `nats:2-linux`

```console
$ docker pull nats@sha256:eb248ee016566129be55f099933db3c2daa1b235a9831eab265fb9b8324cd269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:e6916a74a9af2d54502bfa1459a3e0702c00faa14327b3f3b812262e8ada0966
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4933617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbb0263a71ad823c35b7c360c016e57737a4367ef1c4909a859acb0ddb4ab19a`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:ac560677dbfad917be71a9245045f536b2801212b542bc63c664d6d11156f4dc in /nats-server 
# Tue, 07 Feb 2023 02:43:58 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:43:58 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:43:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:43:59 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:43:59 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:5668bc7ee19e1c51e1510bfeee7245e2b2cc66a8b8f8b0f988f4b3bca8729cec`  
		Last Modified: Tue, 07 Feb 2023 02:44:45 GMT  
		Size: 4.9 MB (4933108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d5b4d77a0e7f6c3fed0f1ae97dbe1b22a3ed4e6af873e7782a0b1d2b992779`  
		Last Modified: Tue, 07 Feb 2023 02:44:44 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:b141eec319986960b56193a2de1a779138beb96cb9945ebc12dbbe199ca96382
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4696311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89f9b13a403b08d651892f330e0f3dd788a5fb00fd1f6338e79860d306d4504d`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:4eee0f78d63bff3b20fac11aaeb64833cd520dac95605f8f9015e670e58a5ef7 in /nats-server 
# Tue, 07 Feb 2023 01:52:41 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:41 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:41 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:41 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6a1ef747dccf7d40d061dc4c857fff9b056d8693e427a2f3adaebc1e22066869`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 4.7 MB (4695803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7ba083439d0caacde0ad211a483925f47f6ec3916cf261abe491ac5a630aaf`  
		Last Modified: Tue, 07 Feb 2023 01:54:10 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:ccb41e1e35bee87bcd6a70e43fd88e284140c67701fb8f639781a7b0b7201eb6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4691076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a4d042e0f28cb5cfa1b6a77c7eb4e06d62ffbfd2c681f2ca2f1aa747dc538cf`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:5f0ce15e9664bd3755e850351446cf7719b19193e891220c68a9776456e2700a in /nats-server 
# Tue, 07 Feb 2023 02:00:54 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 02:00:54 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:00:54 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 02:00:54 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 02:00:54 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:858d33663bc30713d47f7de008a1659f090a1ab8df117e447c1623a289378d31`  
		Last Modified: Tue, 07 Feb 2023 02:02:24 GMT  
		Size: 4.7 MB (4690568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4973a38193b2d039d297077dd1451a47493f724dd8283e465313c615bcbbb8`  
		Last Modified: Tue, 07 Feb 2023 02:02:23 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:1689ba4ea78e52511a025fdbe524cf1d62dc69c0c2bb68119fabb955e8513246
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4519578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96bb932300dca1eb555905232fe9caf2ee65c6b8285cc68e13cf30bb07bd94d3`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:cc453883d11f3e7a77a5f311e510cb07fee2fd66b31eb11f16a5f8023889f08d in /nats-server 
# Tue, 07 Feb 2023 01:52:13 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Tue, 07 Feb 2023 01:52:13 GMT
EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 01:52:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Tue, 07 Feb 2023 01:52:13 GMT
ENTRYPOINT ["/nats-server"]
# Tue, 07 Feb 2023 01:52:13 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:cf0e5763ec64b26f959ef78ac3641929a51a1fda6989adfd65f04af6f8b3a53a`  
		Last Modified: Tue, 07 Feb 2023 01:53:02 GMT  
		Size: 4.5 MB (4519070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb009df287c6f73705947a89031473f06a27171a64409e09c24fc061c1863d5`  
		Last Modified: Tue, 07 Feb 2023 01:53:01 GMT  
		Size: 508.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
