## `hello-world:nanoserver-1809`

```console
$ docker pull hello-world@sha256:99975dac134efe54433a3ad16e0e3c65d5375ea121ec607490682f8a45c732a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4974; amd64

### `hello-world:nanoserver-1809` - windows version 10.0.17763.4974; amd64

```console
$ docker pull hello-world@sha256:e1c66f56cd584a6fc5f939fb8fc357b9c715830605056a9c1a9c9798f7029647
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104467623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d18db4bcd78333c88f5881487d746720eceb250d08a939a96820c8d4fd04ed25`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Mon, 02 Oct 2023 07:48:04 GMT
RUN Apply image 10.0.17763.4974
# Wed, 11 Oct 2023 02:53:19 GMT
RUN cmd /S /C #(nop) COPY file:994f63bc3cea8285310afa5f4677df29bf99dd4cd1881c7e381100a9e794ba71 in C: 
# Wed, 11 Oct 2023 02:53:23 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:5f8edc2588edb9971a52d53cd4265062614ebb25e94063a4d235376797b0e57a`  
		Last Modified: Tue, 10 Oct 2023 17:24:08 GMT  
		Size: 104.5 MB (104464580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c0ef0991d147a381f0927e7a589380073551449c28a6ecabdffedb2f0d877c3`  
		Last Modified: Wed, 11 Oct 2023 02:53:46 GMT  
		Size: 1.9 KB (1884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ac58c0cb712c15a72286fc4f400444677f8c045be918f73da000b869c63370`  
		Last Modified: Wed, 11 Oct 2023 02:53:46 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
