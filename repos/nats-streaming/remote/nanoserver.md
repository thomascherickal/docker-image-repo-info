## `nats-streaming:nanoserver`

```console
$ docker pull nats-streaming@sha256:a8998506db11878d76d6c5852804544f9c8129b9a980fe8c32ff898961a4664f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2061; amd64

### `nats-streaming:nanoserver` - windows version 10.0.17763.2061; amd64

```console
$ docker pull nats-streaming@sha256:349783a72dc891fd56179a54e998371cfe730524625447c5e5f8c8f99ef7d065
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.0 MB (110023666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2c8c7df75f26ed571fde792979a0ab215e1f76ff8e9a7f250cc092b15254741`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 06 Jul 2021 20:06:39 GMT
RUN Apply image 1809-amd64
# Wed, 14 Jul 2021 02:35:24 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Mon, 02 Aug 2021 22:17:13 GMT
RUN cmd /S /C #(nop) COPY file:9670e5d1fe5a71e47c78fde01235a0bcbcafcfdeeacf96a7669f6e49343fb03b in C:\nats-streaming-server.exe 
# Mon, 02 Aug 2021 22:17:16 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Mon, 02 Aug 2021 22:17:18 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Mon, 02 Aug 2021 22:17:21 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:29d43e56445c5279a6386c4dfe4d1ada3c7124ade9cb7b0f2757e58ffc7cd10b`  
		Size: 102.7 MB (102725622 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ec20c4c9f6fa5e782e09342d50033ef24c4049a9dad1befd33c96759b71da6de`  
		Last Modified: Wed, 14 Jul 2021 02:40:36 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395219f11b245d57e94766328eb17b3d461dcfac8402452fdc67df4b9e64361e`  
		Last Modified: Mon, 02 Aug 2021 22:22:03 GMT  
		Size: 7.3 MB (7293366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ed48c75b28949dec2cdb6cb3ff1179ad63c4c4371eba6a69a24baf25f2f6599`  
		Last Modified: Mon, 02 Aug 2021 22:21:54 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9b056cd35fd11d0c1057a2de6be2e533de9455af3383d08143215e972c3fd1`  
		Last Modified: Mon, 02 Aug 2021 22:21:55 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20642618c26e07a2aaf5f4169ff1a42ac92cb50404ebb140d800a9da097779ca`  
		Last Modified: Mon, 02 Aug 2021 22:21:55 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
