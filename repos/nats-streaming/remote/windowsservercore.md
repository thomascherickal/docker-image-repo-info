## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:7b2e0f23e86697455da11923ac1c457308ecb0a3122243ab50ade109481ba51a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3750; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.14393.3750; amd64

```console
$ docker pull nats-streaming@sha256:87f06d59c39b45e75f38497fabcf1e98077530979d9e2992952faf9d481cb97e
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5740054760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b1620beba2f596e6dbbb122b91270a7695fc9b88ec93621502409033ca97b4f`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 01 Jun 2020 18:53:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Jun 2020 18:11:14 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 10 Jun 2020 18:11:16 GMT
RUN cmd /S /C #(nop) WORKDIR C:\nats-streaming-server
# Wed, 10 Jun 2020 18:11:17 GMT
RUN cmd /S /C #(nop) COPY file:d30725f7225d14fba35e88513adf63da18fc9fef9c4f6c817dff8f784f19a7c1 in nats-streaming-server.exe 
# Wed, 10 Jun 2020 18:11:19 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 10 Jun 2020 18:11:20 GMT
RUN cmd /S /C #(nop)  CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:375fbabb84945635805b46a02a17ac15a3177bcaae7404cfab5f1ceb0460cb60`  
		Size: 1.7 GB (1664011795 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:434f1ffc98baa91fed029af9f5559d211024196d545c4b9f27db588a9ad525f6`  
		Last Modified: Wed, 10 Jun 2020 18:11:44 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab81a88c29ec1809fa0486da85779637b2a9d3f72dc80bc871ca1136343d6f13`  
		Last Modified: Wed, 10 Jun 2020 18:11:44 GMT  
		Size: 1.3 KB (1297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005d35c38a49334c8abd805aaaf415ce52a8f4c86d5eb65c6406201eebe86bc5`  
		Last Modified: Wed, 10 Jun 2020 18:11:47 GMT  
		Size: 6.1 MB (6052318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2cee8211b7e9df3250a26f384419f566e9f318b3a961c68ff42960e3b0ff61`  
		Last Modified: Wed, 10 Jun 2020 18:11:45 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e7a523794ca912be576aaae4c74c5133d5b233a5751aa1408f5028da5a21b8`  
		Last Modified: Wed, 10 Jun 2020 18:11:44 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
