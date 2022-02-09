## `hello-world:nanoserver-1809`

```console
$ docker pull hello-world@sha256:94750431ae5b0c3426d1c0cb900ef7dbbcafcba2e68c2349e0cd186d6fbf0104
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2565; amd64

### `hello-world:nanoserver-1809` - windows version 10.0.17763.2565; amd64

```console
$ docker pull hello-world@sha256:fdea2bf76c9a47fc0b81958cb87aa65448012ef36ce051a72a09db398efdf7cc
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.1 MB (103090153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e8e1b8a5e20843f985e78acf03084fa3521b9e943aa559ca81f9800fd05d52e`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Wed, 02 Feb 2022 19:06:51 GMT
RUN Apply image 1809-amd64
# Wed, 09 Feb 2022 13:30:04 GMT
RUN cmd /S /C #(nop) COPY file:dbb4e437ca342a79d5980fcb71c065abfe00353f696b1b54084e7c09d32ec085 in C: 
# Wed, 09 Feb 2022 13:30:05 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:bd0b37167cd3d731eb15196e123df7156b5a35597874d3016a1a4298c46fac3f`  
		Size: 103.1 MB (103087119 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eb6e9f1ba38deddcabe04af2742979555a380548ff92cb86930bd1c01a18667e`  
		Last Modified: Wed, 09 Feb 2022 13:30:27 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c55070d8202fc76c65b80f753b0fe87f79745389271abbdbc460f7fd9749f8`  
		Last Modified: Wed, 09 Feb 2022 13:30:27 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
