## `hello-world:nanoserver-ltsc2022`

```console
$ docker pull hello-world@sha256:fd622ed21df11e914c9f4c3632d5901f187007ecca4e0af816df5a47205015c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.524; amd64

### `hello-world:nanoserver-ltsc2022` - windows version 10.0.20348.524; amd64

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
