## `golang:rc-nanoserver-1809`

```console
$ docker pull golang@sha256:71ddd4fbfbd820cb30833c98fc1a072e18935a40c80e6f062259d6249efbc852
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.973; amd64

### `golang:rc-nanoserver-1809` - windows version 10.0.17763.973; amd64

```console
$ docker pull golang@sha256:8e5399d0fe56674b55b60ac5eecfba199ead21463100046e02a65bd76fd35066
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.0 MB (234038160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:279524f9c686451e467022477ffb82b760f782dc5c6c17233d9fec8ff0a1e5e0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Sat, 04 Jan 2020 07:17:17 GMT
RUN Apply image 1809-amd64
# Wed, 15 Jan 2020 13:30:43 GMT
SHELL [cmd /S /C]
# Wed, 15 Jan 2020 13:30:45 GMT
ENV GOPATH=C:\gopath
# Wed, 15 Jan 2020 13:30:46 GMT
USER ContainerAdministrator
# Wed, 15 Jan 2020 13:31:01 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\go\bin;%PATH%"
# Wed, 15 Jan 2020 13:31:03 GMT
USER ContainerUser
# Thu, 06 Feb 2020 00:34:35 GMT
ENV GOLANG_VERSION=1.14rc1
# Thu, 06 Feb 2020 00:39:36 GMT
COPY dir:cdeb49570d2ca00ee78b13ff980deddada223d70dbc8a88e54511883f52354ef in C:\go 
# Thu, 06 Feb 2020 00:39:54 GMT
RUN go version
# Thu, 06 Feb 2020 00:39:55 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:ee446884f7bef76f8275c2f16add1c4fb598bea2ba861e72bce8fb4aac9b55ef`  
		Size: 101.1 MB (101054324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b6d2b296a71d6933ef11f4e74561e6121347a2ed94dca1fe05411acddda6dee1`  
		Last Modified: Wed, 15 Jan 2020 14:22:06 GMT  
		Size: 915.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655360e4f5b854fc477573e7aa01a5bd2d1a98ab61dc034faf439252c8e5f6bb`  
		Last Modified: Wed, 15 Jan 2020 14:22:06 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a112b2082077143e3991a1c8271eda1759f92aaeed15fc7be7d1833e5a060ce`  
		Last Modified: Wed, 15 Jan 2020 14:22:06 GMT  
		Size: 924.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:080c04b06396990c98c38d890143af9a6095e331d70bdb3fa41e377ccad5011b`  
		Last Modified: Wed, 15 Jan 2020 14:22:06 GMT  
		Size: 67.9 KB (67942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f61b854e0e2419e287db310a75064a06d74adbd4af044d4364108e90defb20`  
		Last Modified: Wed, 15 Jan 2020 14:22:03 GMT  
		Size: 917.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998f1919d77d27ecc0ed7b9096377bdef70d5de545c5641fb94b73526cfa000f`  
		Last Modified: Thu, 06 Feb 2020 00:48:16 GMT  
		Size: 942.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3577a1881dfb6fcff78feec61eea9d591dac9be84ae7da99e539fe029fc10c7`  
		Last Modified: Thu, 06 Feb 2020 00:49:56 GMT  
		Size: 132.9 MB (132869639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda1e2d899aed8c2fc6d22ff9c57b777e52c3967fae8336520533dc8fec28df7`  
		Last Modified: Thu, 06 Feb 2020 00:48:17 GMT  
		Size: 40.4 KB (40447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:029d2dd6dfc0eee559f1a095733c9b8fd4036bf1d7e13b375b28aeb2af62d19a`  
		Last Modified: Thu, 06 Feb 2020 00:48:17 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
