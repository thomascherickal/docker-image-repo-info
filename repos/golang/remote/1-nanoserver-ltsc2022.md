## `golang:1-nanoserver-ltsc2022`

```console
$ docker pull golang@sha256:ddbf88632950e512c49771d54958d770c2f18e8876caa61d0b512e16fd6d2f9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `golang:1-nanoserver-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull golang@sha256:4cd5e6ac290a5d8343c726cab4690a233946db846a224bb952487825c6b98826
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.5 MB (275478844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40cb6b5739fa4c3cdc680f2082fd22c4a298f716a09fbc63ba631869d02b8572`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Sat, 06 Aug 2022 18:05:23 GMT
RUN Apply image 10.0.20348.887
# Wed, 10 Aug 2022 13:00:01 GMT
SHELL [cmd /S /C]
# Wed, 10 Aug 2022 13:00:02 GMT
ENV GOPATH=C:\go
# Wed, 10 Aug 2022 13:00:03 GMT
USER ContainerAdministrator
# Wed, 10 Aug 2022 13:00:52 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Wed, 10 Aug 2022 13:00:53 GMT
USER ContainerUser
# Tue, 06 Sep 2022 19:24:22 GMT
ENV GOLANG_VERSION=1.19.1
# Tue, 06 Sep 2022 19:27:13 GMT
COPY dir:8931e4de46b22c4907fdd32bb2e3bdcb14b258c585caf020889cae248acd1241 in C:\Program Files\Go 
# Tue, 06 Sep 2022 19:28:08 GMT
RUN go version
# Tue, 06 Sep 2022 19:28:09 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:2ebf439f800cd4c1fccaf4a0545e6bff60caa5141295c8ab81f6c525073c423d`  
		Size: 118.1 MB (118088450 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:28bba27fcdd9c2f008a9c22db6c16dece3a5c3a49f9fac9447924071999adf65`  
		Last Modified: Wed, 10 Aug 2022 13:26:19 GMT  
		Size: 1.1 KB (1140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f352dc9aa1911058088d17b0106a92f12440eeeca4743fefe0c8f4341b35cb`  
		Last Modified: Wed, 10 Aug 2022 13:26:19 GMT  
		Size: 1.2 KB (1166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71cdaa41fdd816a0d26ae34d42202146e1c097c5c1f8d4a7e89baa4b6c898e11`  
		Last Modified: Wed, 10 Aug 2022 13:26:18 GMT  
		Size: 1.1 KB (1116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de3ee36144ab0c42283d413099bae19e983ae4415ed4f3aadf1b2f00dee77af`  
		Last Modified: Wed, 10 Aug 2022 13:26:19 GMT  
		Size: 85.0 KB (85027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd92736439907ce6bf37d9c346db5466b4a71f29695648b075e599df34b709b2`  
		Last Modified: Wed, 10 Aug 2022 13:26:16 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef41a4e2a0f3e16498f1bb0d1594baa0cdfaf6e77443d1477ccff33c32aa0c5`  
		Last Modified: Tue, 06 Sep 2022 19:50:21 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af9b83eb420c08497ed8361afa59c768b46c507c19a256aae4e93014f786912`  
		Last Modified: Tue, 06 Sep 2022 19:50:58 GMT  
		Size: 157.2 MB (157246445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bda2a58e8412c469d40a83a9109f712fe85e138cea8ed7fb7855abe7f29bcb0`  
		Last Modified: Tue, 06 Sep 2022 19:50:21 GMT  
		Size: 51.9 KB (51852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d301a857e784690c1f0651458e018f02f6446e9163446ec0090bc1000d48cb7`  
		Last Modified: Tue, 06 Sep 2022 19:50:21 GMT  
		Size: 1.4 KB (1360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
