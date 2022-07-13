## `hello-world:nanoserver-1809`

```console
$ docker pull hello-world@sha256:5103872ae58dbb0f1384683764664030fc5dcabefd01d3db0bbcc133a7ef1ff5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `hello-world:nanoserver-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull hello-world@sha256:90baaa24dd546f7d73c33830e849c1d9298d3699c150eb823d13737a49de6503
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.2 MB (103158004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17355e81ee5faeabab9e50b541b40544de8aa52c23e9afea68463f76d985bf1e`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Wed, 06 Jul 2022 22:15:10 GMT
RUN Apply image 10.0.17763.3165
# Wed, 13 Jul 2022 12:40:02 GMT
RUN cmd /S /C #(nop) COPY file:994f63bc3cea8285310afa5f4677df29bf99dd4cd1881c7e381100a9e794ba71 in C: 
# Wed, 13 Jul 2022 12:40:02 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:5d24e1a2f5c566b0afb1e46fc24e5cec821c8ebf44220276a95a2b91f44a2f2a`  
		Size: 103.2 MB (103155009 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:03026d78c06d34b0656e93ecf231173dcee8f5e95f4644c436c119761538a2aa`  
		Last Modified: Wed, 13 Jul 2022 12:40:25 GMT  
		Size: 1.9 KB (1865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5af39094b906c69d1b8e28abf692dba17b2f360bc746d7915cd0052f56e7dd5`  
		Last Modified: Wed, 13 Jul 2022 12:40:25 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
