## `hello-world:nanoserver-1809`

```console
$ docker pull hello-world@sha256:671f3e58d6f61beaa86a412241fdde1797028cd09199662f2654826da384c285
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `hello-world:nanoserver-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull hello-world@sha256:141da54de860ac576d546afeed7c0e3df1d7eac32ae547b50032e88da2699361
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106674043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f08cff1de62a32925d8d542754de47dce241ff2640e1d9b48bbd3f064c542a03`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Sun, 11 Dec 2022 07:45:27 GMT
RUN Apply image 10.0.17763.3770
# Wed, 14 Dec 2022 01:24:33 GMT
RUN cmd /S /C #(nop) COPY file:994f63bc3cea8285310afa5f4677df29bf99dd4cd1881c7e381100a9e794ba71 in C: 
# Wed, 14 Dec 2022 01:24:34 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:7442c6014cd8a0820e2009cde1268b6ce4b8f86bc314ba287cc01fab93174fd6`  
		Last Modified: Tue, 13 Dec 2022 23:57:28 GMT  
		Size: 106.7 MB (106671057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18e8f77eaf07ea6f526a6fe86427fbd6bab1a26cac7b80224a821ab088d54b0`  
		Last Modified: Wed, 14 Dec 2022 01:24:58 GMT  
		Size: 1.8 KB (1848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d556b4fbb745283ade6bf650bbe9ec2653957513dc0f1397f047394a8e3eeb1`  
		Last Modified: Wed, 14 Dec 2022 01:24:58 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
