## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:0c8235955eaa45abc0c19f1d81824bf5a1d16988a903b18e316fa24776112b19
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull nats-streaming@sha256:eebe09377a3efa612c603d6fedad843e422597e22fcf570cc8d7708f326c0199
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106567957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aec57a1f1252a3a6c4774b55f39871e60d7af96178ff2a3a8473cdd011b54dd8`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 04 Jan 2020 07:17:17 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jan 2020 17:50:29 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 21:35:36 GMT
RUN cmd /S /C #(nop) WORKDIR C:\nats-streaming-server
# Wed, 15 Jan 2020 21:35:39 GMT
RUN cmd /S /C #(nop) COPY file:d333dfb9aa0fca02ce2e2300447082af645803b49703ee1671951f7dba266042 in nats-streaming-server.exe 
# Wed, 15 Jan 2020 21:35:41 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 15 Jan 2020 21:35:42 GMT
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
	-	`sha256:efe2410e2bf1317b29002d506dc0eb4ed7871159d2826be76277d8ab2e54abac`  
		Last Modified: Wed, 15 Jan 2020 21:37:03 GMT  
		Size: 5.5 MB (5509664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be23e3b723ccca3ca67b599804e78000ac64ab92db764d3c8a791d6ddfc9a374`  
		Last Modified: Wed, 15 Jan 2020 21:37:01 GMT  
		Size: 928.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1b881d4c2144a0226571a3ca15876983ff65f65e163f7aa6ea4ccafa0cf420`  
		Last Modified: Wed, 15 Jan 2020 21:37:01 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
