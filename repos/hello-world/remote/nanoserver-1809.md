## `hello-world:nanoserver-1809`

```console
$ docker pull hello-world@sha256:2042583887a6cb63ce428aa792258b8f72965bdab285aabf3d3c009443cab6d2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1158; amd64

### `hello-world:nanoserver-1809` - windows version 10.0.17763.1158; amd64

```console
$ docker pull hello-world@sha256:093df2ad7845fff954aba49fed9c63ed09bfe280706cd849402aab9314982437
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.1 MB (101120871 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7f4e41fba3a1f17ca2f9470632fcbb9aa465942cf2132529bfacc5196be404b`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Sun, 12 Apr 2020 11:41:03 GMT
RUN Apply image 1809-amd64
# Wed, 15 Apr 2020 12:13:06 GMT
RUN cmd /S /C #(nop) COPY file:0afaffc2fa64462107b7178b2ae7d20404ff12f637eabe3a8046192b9d9a0338 in C: 
# Wed, 15 Apr 2020 12:13:07 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:0fe89239909ba300aeb9b977458b61ae3fbbcd2d9591086ed05ca023209d3122`  
		Size: 101.1 MB (101118377 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d5764f3a7b3b769a6ca788acd207dd1c3d48e1968bb66e7b17f122a03455645b`  
		Last Modified: Wed, 15 Apr 2020 12:13:18 GMT  
		Size: 1.6 KB (1602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48f3724e92bb02e0ec42a5d0fd347e37d3ed8b55ddf9e19b76f26857e4256f2`  
		Last Modified: Wed, 15 Apr 2020 12:13:18 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
