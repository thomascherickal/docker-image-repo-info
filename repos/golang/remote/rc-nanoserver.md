## `golang:rc-nanoserver`

```console
$ docker pull golang@sha256:16a2e3610f44b22941722eb052ef5cb92ce545477cb2e12b1a4990c4dadacee0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17134.950; amd64
	-	windows version 10.0.17763.678; amd64

### `golang:rc-nanoserver` - windows version 10.0.17134.950; amd64

```console
$ docker pull golang@sha256:f57f5e30642b02d2361096a1d21daa1c25bfdc3136c2367bf940a303f3cd3a49
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **280.1 MB (280149536 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcb0a30438ae293ac7e1d3812ea28e8e256e6d7e7e37b8b31faa747ccbeb7f9e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Wed, 11 Apr 2018 22:12:30 GMT
RUN Apply image 1803-RTM-amd64
# Fri, 09 Aug 2019 14:57:28 GMT
RUN Install update 1803-amd64
# Tue, 13 Aug 2019 23:57:01 GMT
SHELL [cmd /S /C]
# Tue, 13 Aug 2019 23:57:02 GMT
ENV GOPATH=C:\gopath
# Tue, 13 Aug 2019 23:57:04 GMT
USER ContainerAdministrator
# Tue, 13 Aug 2019 23:57:20 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\go\bin;%PATH%"
# Tue, 13 Aug 2019 23:57:21 GMT
USER ContainerUser
# Thu, 29 Aug 2019 21:46:55 GMT
ENV GOLANG_VERSION=1.13rc2
# Thu, 29 Aug 2019 21:51:53 GMT
COPY dir:3a8623148a45b3ef72a14ba7336374fb856fa64a828b11e45f3208504c35c3c8 in C:\go 
# Thu, 29 Aug 2019 21:52:13 GMT
RUN go version
# Thu, 29 Aug 2019 21:52:14 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:e46172273a4e4384e1eec7fb01091c828a256ea0f87b30f61381fba9bc511371`  
		Last Modified: Mon, 17 Sep 2018 20:23:30 GMT  
		Size: 92.8 MB (92818888 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a41df37ffdede5c4ccd6634c1d787effb06f3600d661aea6e29d326dd6d36bad`  
		Last Modified: Fri, 09 Aug 2019 15:39:33 GMT  
		Size: 58.0 MB (57977516 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dd3ca2ada7ad1bb25def26ca5cb9ff4556c5c668ad1642a5c5ebc474e74a670d`  
		Last Modified: Wed, 14 Aug 2019 01:11:18 GMT  
		Size: 917.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6200fb9fe7661aaeca009adf883084cf351824b61bd19e0aa24e798cf439cc7`  
		Last Modified: Wed, 14 Aug 2019 01:11:18 GMT  
		Size: 927.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6783d058769a6632e954ed7f04858dc6b4567c32c19f5c42eac4a2104c7cea54`  
		Last Modified: Wed, 14 Aug 2019 01:11:18 GMT  
		Size: 921.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3543c27618ab7cb1737aa0f8d97f45df5272858798e5fe7300e14dcb8e2f5c2`  
		Last Modified: Wed, 14 Aug 2019 01:11:18 GMT  
		Size: 69.1 KB (69134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43976f23d0193c48f5c31e308819ff164a18ff83ff45eac737413c9ca20129fa`  
		Last Modified: Wed, 14 Aug 2019 01:11:16 GMT  
		Size: 939.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32afa5db4ad1bb413b94b1dc43e29c8285fb3166a2dd72a3276416a57e65e16`  
		Last Modified: Thu, 29 Aug 2019 22:06:33 GMT  
		Size: 915.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f03993fab6d976426bd474a4d4df228fbb8a1260bda6064e9a3f70137048da`  
		Last Modified: Thu, 29 Aug 2019 22:09:51 GMT  
		Size: 129.2 MB (129237079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0f51a35f2f0d1a6a0d1d4c3f99ce9775486d20ff99a2618a99c8cc9fbbf2c4`  
		Last Modified: Thu, 29 Aug 2019 22:06:33 GMT  
		Size: 41.1 KB (41129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c50dfd4ccbf05dbb8728aa239052b38b53733c7adb3e30a1dae8b65ae5282f`  
		Last Modified: Thu, 29 Aug 2019 22:06:33 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:rc-nanoserver` - windows version 10.0.17763.678; amd64

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
