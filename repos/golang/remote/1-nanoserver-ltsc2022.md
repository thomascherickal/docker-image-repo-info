## `golang:1-nanoserver-ltsc2022`

```console
$ docker pull golang@sha256:522bf6a5ce5f2dd0c5ef54bdb8f7ccb8558c5d6d7108ba3c24e9896e4aad0fbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1249; amd64

### `golang:1-nanoserver-ltsc2022` - windows version 10.0.20348.1249; amd64

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
