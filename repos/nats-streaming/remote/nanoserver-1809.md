## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:f8ed57ea03af970af3e4adebc240f65b9d4c0245ce09c2cab2afd188fdfbe081
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats-streaming@sha256:384c62d23f7a6591a1a30e469740d7f389faba17231c0420240e12798c31142a
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107110462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f4abd48c3c9c23c675497fcb59c7414990f34f0a056389f77ef153692b74a29`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 04 Jan 2020 07:17:17 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jan 2020 17:50:29 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 21:35:36 GMT
RUN cmd /S /C #(nop) WORKDIR C:\nats-streaming-server
# Fri, 14 Feb 2020 00:23:01 GMT
RUN cmd /S /C #(nop) COPY file:d30725f7225d14fba35e88513adf63da18fc9fef9c4f6c817dff8f784f19a7c1 in nats-streaming-server.exe 
# Fri, 14 Feb 2020 00:23:03 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 14 Feb 2020 00:23:04 GMT
RUN cmd /S /C #(nop)  CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:ee446884f7bef76f8275c2f16add1c4fb598bea2ba861e72bce8fb4aac9b55ef`  
		Size: 101.1 MB (101054324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95d31e7189792498b758db35ae56b1ca97128d8063404cbe62a32205d08d1d4a`  
		Last Modified: Wed, 15 Jan 2020 17:54:30 GMT  
		Size: 940.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67d663157e963f00f643c894608331692ddb1c32c25e3d420817b35f71844785`  
		Last Modified: Wed, 15 Jan 2020 21:37:01 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83968c872fa4dd50515740d84ca5e01213df13bf7246e335a13f7da4301515b0`  
		Last Modified: Fri, 14 Feb 2020 00:23:53 GMT  
		Size: 6.1 MB (6052161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58edd96e534fce213e5123cc71ec302c157bc8c202d6017f720948442d9283bb`  
		Last Modified: Fri, 14 Feb 2020 00:23:51 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a4a512a51dd6bb1dc246ac0dcc2a0f3fbd8f0968c3751f4640719994d25c54`  
		Last Modified: Fri, 14 Feb 2020 00:23:51 GMT  
		Size: 938.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
