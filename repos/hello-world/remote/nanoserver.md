## `hello-world:nanoserver`

```console
$ docker pull hello-world@sha256:6cc40041f94d0d9a498d5a1b10cb4f6154c57e33f05ce8739e0e3d8ed985b13c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1518; amd64

### `hello-world:nanoserver` - windows version 10.0.17763.1518; amd64

```console
$ docker pull hello-world@sha256:73de1a34e3ed861361a58431f33f309f0f8ca608bea88b70e6046feaa5cf0fd0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.2 MB (101207621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8089101ead9ce9b8c68d6859995c98108e1022c23beaa55754acb89d66fd3381`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Wed, 30 Sep 2020 11:25:56 GMT
RUN Apply image 1809-amd64
# Wed, 14 Oct 2020 12:12:26 GMT
RUN cmd /S /C #(nop) COPY file:0afaffc2fa64462107b7178b2ae7d20404ff12f637eabe3a8046192b9d9a0338 in C: 
# Wed, 14 Oct 2020 12:12:27 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:aab6118ce69c93410df7fa15842a6e3b3c7ff20b639c779b5d5f78e7653eaa07`  
		Size: 101.2 MB (101205155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b9c1b122ed958fbeaf2f62867f9fd16013fe461d688b39989453f0d83c462c46`  
		Last Modified: Wed, 14 Oct 2020 12:12:39 GMT  
		Size: 1.6 KB (1603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8e5afdd0c113a582983ad874038f14db4d53a3b3ef17ca6108afe401378834`  
		Last Modified: Wed, 14 Oct 2020 12:12:39 GMT  
		Size: 863.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
