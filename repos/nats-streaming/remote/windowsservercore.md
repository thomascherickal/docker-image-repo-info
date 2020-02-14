## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:344316b8755e5d34362fe5261d866d82dba1224407fcea3a27b86642b65f1afd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3443; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.14393.3443; amd64

```console
$ docker pull nats-streaming@sha256:c0a18fb14f3453956b68bed2c033b47c2424aed8141d41f2a7ee32662d07c430
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5730656577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeb7701e54a62125672efe5ddeb43758bedfc00c09eaa11291db37d4cdef5581`
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
# Fri, 14 Feb 2020 00:23:24 GMT
RUN cmd /S /C #(nop) COPY file:d30725f7225d14fba35e88513adf63da18fc9fef9c4f6c817dff8f784f19a7c1 in nats-streaming-server.exe 
# Fri, 14 Feb 2020 00:23:26 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Fri, 14 Feb 2020 00:23:28 GMT
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
	-	`sha256:200e9bf973bb638312456a7b482d1fa9eae9ce04ec45954ed70a11ba6ba80a6a`  
		Last Modified: Fri, 14 Feb 2020 00:24:19 GMT  
		Size: 6.1 MB (6052353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:538e6b439628ec2e6f0fec79407f21151754f8ca48903dd7040a3ef88ce30dbb`  
		Last Modified: Fri, 14 Feb 2020 00:24:17 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a90b22fe2290ad1fb16f63b4e5e5efaa5437bec23ec9b5650492dd86a61d00e`  
		Last Modified: Fri, 14 Feb 2020 00:24:18 GMT  
		Size: 1.2 KB (1205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
