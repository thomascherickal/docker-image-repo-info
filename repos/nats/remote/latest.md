## `nats:latest`

```console
$ docker pull nats@sha256:f80a2e0337ac068122897636f9f6d686a397ea56f593e0ce0a603cdf41e6e027
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.3887; amd64

### `nats:latest` - linux; amd64

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

### `nats:latest` - linux; arm variant v6

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

### `nats:latest` - linux; arm variant v7

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

### `nats:latest` - linux; arm64 variant v8

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

### `nats:latest` - windows version 10.0.17763.3887; amd64

```console
$ docker pull nats@sha256:e6a17bb97fb6a291a4bd98d30c3b9099dedbcf70d12fb062efebaabdb1213bbc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.7 MB (111659596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45804cd0005e5185373d2c577a4257391cd004c68b4c440f4678cf10382b2db7`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Sat, 07 Jan 2023 05:17:01 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 05:01:51 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Tue, 07 Feb 2023 02:18:03 GMT
RUN cmd /S /C #(nop) COPY file:a45a34d252c029bb58fb3b3e2b3592a2d7869806250714c7b6dc3fb0b305c7bd in C:\nats-server.exe 
# Tue, 07 Feb 2023 02:18:04 GMT
RUN cmd /S /C #(nop) COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Tue, 07 Feb 2023 02:18:05 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Tue, 07 Feb 2023 02:18:06 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:e58f9ad3b15a2a4882ab0a845e8e619cc8c3c411ddbe8b50046c1618a95c1397`  
		Last Modified: Thu, 12 Jan 2023 02:40:44 GMT  
		Size: 106.7 MB (106666138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe88f4c5f9972ffecb9a66b92e75ddfe48bf7d8d451ace7af3527653f67ff9e`  
		Last Modified: Thu, 12 Jan 2023 05:02:42 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6572a3c131299689497339cc59b098f3601ad482ac0828eeaba7e5f78dc21d76`  
		Last Modified: Tue, 07 Feb 2023 02:18:55 GMT  
		Size: 5.0 MB (4987024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5a625d40bd2eadd9e49c606bd8fad79a2aa73ebcd3313c3de00a12b06738c7`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.8 KB (1788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9650a5245dfd33f33fb4a5df832057f9d0b34cb3febe41b20095202eda9b58f`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ca02e3d157746bd7381b47df24d65195a307dadd09eba9a311c95481d51b4d`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd2be7007de85b1c3f78a02ae15fdfcf679c7378b8d53403ebe90f39cd16418`  
		Last Modified: Tue, 07 Feb 2023 02:18:53 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
