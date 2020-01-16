## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:851279675835541cd5bfa73bb185acd88eec08813b3e74bf53bd2e78b365ffc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3443; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.14393.3443; amd64

```console
$ docker pull nats-streaming@sha256:39bfa1f861057c49ed2197289cbf770b5807257f0356ff0cb60252d0a29df96b
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5730114269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:574a3bb951d80f6383434ed1065d07f98a4fca660cc8eebf1ea2a464ba4c735f`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jan 2020 21:35:55 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 15 Jan 2020 21:35:56 GMT
RUN cmd /S /C #(nop) WORKDIR C:\nats-streaming-server
# Wed, 15 Jan 2020 21:35:59 GMT
RUN cmd /S /C #(nop) COPY file:d333dfb9aa0fca02ce2e2300447082af645803b49703ee1671951f7dba266042 in nats-streaming-server.exe 
# Wed, 15 Jan 2020 21:36:01 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 15 Jan 2020 21:36:03 GMT
RUN cmd /S /C #(nop)  CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f292bd4ebcdd092db3cbfe8d43378724110b9e4afc178f8f9ba9a901b76c0fbb`  
		Last Modified: Wed, 15 Jan 2020 21:37:28 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:711e82010a66928ee94c8d73fdc4e9fe8afdee491181e233bb927559ed4b1edc`  
		Last Modified: Wed, 15 Jan 2020 21:37:28 GMT  
		Size: 1.4 KB (1367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f15864b7b4ed2aa3fd79ed4f095a3ad5e53d50702e52456bb6eff7d5e7b79ef3`  
		Last Modified: Wed, 15 Jan 2020 21:37:30 GMT  
		Size: 5.5 MB (5510066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d155fe1c07e390ef051d2c18df499a4bfc91f63ed4a43099911f37c914b24f44`  
		Last Modified: Wed, 15 Jan 2020 21:37:29 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df8a95741d43e2f23a55be93daca653576145a07f3579de191138d5943cee33`  
		Last Modified: Wed, 15 Jan 2020 21:37:28 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
