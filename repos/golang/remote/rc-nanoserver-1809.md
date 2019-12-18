## `golang:rc-nanoserver-1809`

```console
$ docker pull golang@sha256:93aee4fc87721a5c1b3ee874c957c0c79502e06776f0a82bf40c54f061a2aaf8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.678; amd64

### `golang:rc-nanoserver-1809` - windows version 10.0.17763.678; amd64

```console
$ docker pull golang@sha256:5c8b8f2c4fea2521385a7d62b1109dd9c8d3e208f7ba9d17266905d06c2796c1
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **229.8 MB (229767536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e0ae39af2fca6c8f5e09ba20a1e7a11721211b1a58318f985d59b6008360ee34`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Wed, 07 Aug 2019 15:07:45 GMT
RUN Apply image 1809-amd64
# Wed, 14 Aug 2019 00:02:32 GMT
SHELL [cmd /S /C]
# Wed, 14 Aug 2019 00:02:33 GMT
ENV GOPATH=C:\gopath
# Wed, 14 Aug 2019 00:02:35 GMT
USER ContainerAdministrator
# Wed, 14 Aug 2019 00:02:50 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\go\bin;%PATH%"
# Wed, 14 Aug 2019 00:02:51 GMT
USER ContainerUser
# Thu, 29 Aug 2019 21:52:27 GMT
ENV GOLANG_VERSION=1.13rc2
# Thu, 29 Aug 2019 21:57:29 GMT
COPY dir:3a8623148a45b3ef72a14ba7336374fb856fa64a828b11e45f3208504c35c3c8 in C:\go 
# Thu, 29 Aug 2019 21:57:46 GMT
RUN go version
# Thu, 29 Aug 2019 21:57:47 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:85bcf813f547ea541f45281e987b5006b02919ed404f96d666d30402bfcf1f85`  
		Last Modified: Fri, 09 Aug 2019 17:25:04 GMT  
		Size: 100.4 MB (100419796 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d79c2e1befcf34f5b7f2ac8adfc623803cf3acd705556c163d62da8e79980b07`  
		Last Modified: Wed, 14 Aug 2019 01:13:11 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a3c5f6600369d2b3d0b720810602fc773860496dcb5e16793d214710919ad`  
		Last Modified: Wed, 14 Aug 2019 01:13:11 GMT  
		Size: 951.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bf23ffda98fdbe830152e59f66d30386a06d2b7157b44d21c3b3cda0483ba8`  
		Last Modified: Wed, 14 Aug 2019 01:13:11 GMT  
		Size: 949.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310fe6f703adbc601957f7cb279eccfd567bb1e2ed93c910bf32ebc9560aded8`  
		Last Modified: Wed, 14 Aug 2019 01:13:11 GMT  
		Size: 68.1 KB (68115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b47772ce0be967fccf9c4034c3a71781a3133cbb0880f01d839ee3af51349c`  
		Last Modified: Wed, 14 Aug 2019 01:13:09 GMT  
		Size: 899.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3783fe542dc2a0d584123aa84b0ee830c07d5153ed4a8421b01a47e712c01802`  
		Last Modified: Thu, 29 Aug 2019 22:13:34 GMT  
		Size: 918.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3826d42f0ceff874a954ad6f90cafcf8122579a99ca924b6362fcf91b812f6b3`  
		Last Modified: Thu, 29 Aug 2019 22:15:06 GMT  
		Size: 129.2 MB (129237440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e828bc30f494b49edf4e2dfe988984cfcd5fb9f13a285e65ecdc4c54a725a8c3`  
		Last Modified: Thu, 29 Aug 2019 22:13:34 GMT  
		Size: 36.4 KB (36368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:605b30cf195722aae648093e3a242c79a0c1dd405446e4675bf35fd5ecccb49f`  
		Last Modified: Thu, 29 Aug 2019 22:13:34 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
