## `hello-world:nanoserver-1809`

```console
$ docker pull hello-world@sha256:820bed662aecfabf016e20e6c145968a46098ff0055f72dbf41f1da5978a8e22
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `hello-world:nanoserver-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull hello-world@sha256:b0408a0f1d74eced127a2658429f336ed8fa48e36d59878f155b19865e5dbd70
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.4 MB (101393013 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:545e4e38d9db3fd6d543f0b4498a83e91f17166ed9280830a84f984cf22a0149`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Fri, 26 Feb 2021 16:47:31 GMT
RUN Apply image 1809-amd64
# Wed, 10 Mar 2021 13:26:19 GMT
RUN cmd /S /C #(nop) COPY file:dbb4e437ca342a79d5980fcb71c065abfe00353f696b1b54084e7c09d32ec085 in C: 
# Wed, 10 Mar 2021 13:26:20 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:a11c4ca8f1ba16b6e1395d4523be2215bd0871c2e3e4695b9f2b87bd7472be52`  
		Size: 101.4 MB (101389964 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b70d36b981c5bce88c8132b2a7248b435709cf03477d08e8e7f3752cc9f0eaa6`  
		Last Modified: Wed, 10 Mar 2021 13:26:35 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d76481af78e2b81f9ea02fc66c1950cf204cbb93cd49fd1751695d62ec81d9f9`  
		Last Modified: Wed, 10 Mar 2021 13:26:35 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
