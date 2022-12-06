## `golang:nanoserver`

```console
$ docker pull golang@sha256:50142257eb04ae2b1506ebbf30b71fe7f9eef9f7d23a7ac89c431390c686a183
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1249; amd64
	-	windows version 10.0.17763.3650; amd64

### `golang:nanoserver` - windows version 10.0.20348.1249; amd64

```console
$ docker pull golang@sha256:ef771002d183d60b134f690e3e7be9733a63c661b1d56a88dbaa282aff1972db
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.6 MB (279558927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:476ad9258109861ea3cbdddbe522ba39bf9c57533d75fdae5b611f4640e5b339`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Sat, 05 Nov 2022 07:21:30 GMT
RUN Apply image 10.0.20348.1249
# Wed, 09 Nov 2022 14:03:51 GMT
SHELL [cmd /S /C]
# Wed, 09 Nov 2022 14:03:52 GMT
ENV GOPATH=C:\go
# Wed, 09 Nov 2022 14:03:53 GMT
USER ContainerAdministrator
# Wed, 09 Nov 2022 14:04:46 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 09 Nov 2022 14:04:47 GMT
USER ContainerUser
# Tue, 06 Dec 2022 21:22:34 GMT
ENV GOLANG_VERSION=1.19.4
# Tue, 06 Dec 2022 21:25:21 GMT
COPY dir:2cd450fd2156a5a74a4e4b1dc7a490c2568a41af5e46c584b0660f27917680aa in C:\Program Files\Go 
# Tue, 06 Dec 2022 21:26:16 GMT
RUN go version
# Tue, 06 Dec 2022 21:26:17 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:72e5d750fe8c1a32d4a26ef3b4a4e1f6124ac079b142f12724af2abfcba1c8b3`  
		Last Modified: Tue, 08 Nov 2022 19:57:58 GMT  
		Size: 122.1 MB (122092167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5798382a92edbf13363f09d29194b10dba5ce50456d5499d8b33a42e2c702cd`  
		Last Modified: Wed, 09 Nov 2022 14:34:17 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbf23e2a6d8c8cdd8b08934f9eb4c89e5f14495e8dbbebbd9f36eaf8499c66fa`  
		Last Modified: Wed, 09 Nov 2022 14:34:17 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca84d8fc4d105987193f272695a118563c7ba66f1eb720fc4290458642936f81`  
		Last Modified: Wed, 09 Nov 2022 14:34:17 GMT  
		Size: 1.0 KB (1031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ae1bcb3101057a6c0d44e2c647c59153ed3a73922db80c0ae9ef9b392989696`  
		Last Modified: Wed, 09 Nov 2022 14:34:17 GMT  
		Size: 85.7 KB (85698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1f4f26fc0a0987b596c85323510a4c8e97018b9f744605223caf233897f630`  
		Last Modified: Wed, 09 Nov 2022 14:34:14 GMT  
		Size: 1.1 KB (1053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c001964cc68e0b5f3b3e1fd3a412d0708f76dce62ffc08e5ee7ce266c87723`  
		Last Modified: Tue, 06 Dec 2022 21:48:04 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90fdf5f61c71978df0bc503f8b1271fc12e14ded62616e10be4c72e2f9693ad`  
		Last Modified: Tue, 06 Dec 2022 21:48:40 GMT  
		Size: 157.3 MB (157325375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0dd50e08d132296ae83c29bd0ef5e1d66ce24ca2349511f2565c27afd8a3567`  
		Last Modified: Tue, 06 Dec 2022 21:48:04 GMT  
		Size: 48.7 KB (48724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b1ae311872c88d7f13421667de18fc9b116c9fe62afc3bc9cf7e07fd84e137e`  
		Last Modified: Tue, 06 Dec 2022 21:48:04 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:nanoserver` - windows version 10.0.17763.3650; amd64

```console
$ docker pull golang@sha256:187d41e6a419360f8a8e717b827a318d8a97b99d58e3e32935c3eebaa2205b82
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **264.2 MB (264213600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8df931775ee0476be147a003780879623258d7c0833dfd1959cf414a1083eb6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Sat, 05 Nov 2022 18:06:28 GMT
RUN Apply image 10.0.17763.3650
# Wed, 09 Nov 2022 14:09:15 GMT
SHELL [cmd /S /C]
# Wed, 09 Nov 2022 14:09:16 GMT
ENV GOPATH=C:\go
# Wed, 09 Nov 2022 14:09:17 GMT
USER ContainerAdministrator
# Wed, 09 Nov 2022 14:09:59 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 09 Nov 2022 14:10:00 GMT
USER ContainerUser
# Tue, 06 Dec 2022 21:26:35 GMT
ENV GOLANG_VERSION=1.19.4
# Tue, 06 Dec 2022 21:29:10 GMT
COPY dir:2cd450fd2156a5a74a4e4b1dc7a490c2568a41af5e46c584b0660f27917680aa in C:\Program Files\Go 
# Tue, 06 Dec 2022 21:29:56 GMT
RUN go version
# Tue, 06 Dec 2022 21:29:57 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:35ab4104a4d9df6a0d1eac84cc8fbc13511ef6c8aef5ced04fdf63e7e20803a3`  
		Last Modified: Tue, 08 Nov 2022 19:45:20 GMT  
		Size: 106.7 MB (106723592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83e42a06a19f2d133476fa58d61bf56ed65a782146e4f8b37b3fc8727440fbd`  
		Last Modified: Wed, 09 Nov 2022 14:35:26 GMT  
		Size: 1.2 KB (1174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d5f782c7567ec2c9cf757def907e4a540324f1214e9d33dba05ce0c41f3117`  
		Last Modified: Wed, 09 Nov 2022 14:35:26 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67651bffb2b07a227838e94750adbf37f15fe0f26d209f1e80f34f6e508077cf`  
		Last Modified: Wed, 09 Nov 2022 14:35:26 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba67c7baacb632dceb9b260126dcd011a1bdd570f6068decca6106fd87f9cd0`  
		Last Modified: Wed, 09 Nov 2022 14:35:25 GMT  
		Size: 77.1 KB (77078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1daf5190bbe54c04de26fde1d8743bbed1573873c68606a4eee93cd6ff162a3f`  
		Last Modified: Wed, 09 Nov 2022 14:35:23 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ffb10ca6875ff8ec9152a15eed81e0116cb9e13c6915f9800815af290ada76`  
		Last Modified: Tue, 06 Dec 2022 21:48:52 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e10f3be40324f5112cf11b4201284da5a4ea62ac4866bc15eb3b33dd433884`  
		Last Modified: Tue, 06 Dec 2022 21:49:29 GMT  
		Size: 157.3 MB (157328115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06cb053b7bce6fbe9028983a81bcc76bf541bbfca14df0a030b97deb4e1e9288`  
		Last Modified: Tue, 06 Dec 2022 21:48:53 GMT  
		Size: 77.6 KB (77615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7245e5c695693ee3c79f3474f1546d88d5d6b1749150f9603247ff746ca546df`  
		Last Modified: Tue, 06 Dec 2022 21:48:53 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
