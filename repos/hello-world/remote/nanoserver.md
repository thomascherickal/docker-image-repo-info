## `hello-world:nanoserver`

```console
$ docker pull hello-world@sha256:92f0e6447a24c084d2509e6691bd124db4e602077a9ccba010eff7ed1e75bbe5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.524; amd64
	-	windows version 10.0.17763.2565; amd64

### `hello-world:nanoserver` - windows version 10.0.20348.524; amd64

```console
$ docker pull hello-world@sha256:b3dd41b5fbccbf0e39bee932466d389214cddcb53fa4ad5d02f29ee4172db8c7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.5 MB (117460673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b1c4e973c66f52e99dc1baae32ef875bd5f6b8c6000310bacbe3c5733b3b66b`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Tue, 01 Feb 2022 02:25:40 GMT
RUN Apply image ltsc2022-amd64
# Wed, 09 Feb 2022 13:29:59 GMT
RUN cmd /S /C #(nop) COPY file:55c009fa8b983e38026b41064e5367bc779dae76c0d404a11886c3cb19ec4509 in C: 
# Wed, 09 Feb 2022 13:29:59 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:3ab33c1d9cc1eaef56d5617b87373ead45d8a4ff7ab7da384afe612ba569a524`  
		Size: 117.5 MB (117457656 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8e16d6c43d48d5c624643cbd5f4b92bd2d412142a9bf48c30e857c46d8544e00`  
		Last Modified: Wed, 09 Feb 2022 13:30:21 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548223910c2d305a4a5956ba4c81a6800bfc8815359233535e4815218d4b6374`  
		Last Modified: Wed, 09 Feb 2022 13:30:21 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hello-world:nanoserver` - windows version 10.0.17763.2565; amd64

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
