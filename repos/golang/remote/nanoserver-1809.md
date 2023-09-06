## `golang:nanoserver-1809`

```console
$ docker pull golang@sha256:6b927b0df0d569e03d304989a3209d9fa1df0b28a6cb3d03544a9a7fc3810204
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4737; amd64

### `golang:nanoserver-1809` - windows version 10.0.17763.4737; amd64

```console
$ docker pull golang@sha256:05d29c014e633b60b7364e6b7b62edae0c9caf185c935294440968e5af8207e0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.7 MB (173676482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cc22a6130fdb8622e980b2706fff25645bb759c8f4956ca961a03b0ea6d90a1`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Wed, 02 Aug 2023 08:33:47 GMT
RUN Apply image 10.0.17763.4737
# Thu, 10 Aug 2023 00:48:08 GMT
SHELL [cmd /S /C]
# Thu, 10 Aug 2023 00:48:09 GMT
ENV GOPATH=C:\go
# Thu, 10 Aug 2023 00:48:10 GMT
USER ContainerAdministrator
# Thu, 10 Aug 2023 00:48:22 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\Program Files\Go\bin;%PATH%"
# Thu, 10 Aug 2023 00:48:23 GMT
USER ContainerUser
# Wed, 06 Sep 2023 18:39:09 GMT
ENV GOLANG_VERSION=1.21.1
# Wed, 06 Sep 2023 18:40:52 GMT
COPY dir:be682b819fc6157c5849876d4d281ecc9c26fd804e58407c442594a19c48910f in C:\Program Files\Go 
# Wed, 06 Sep 2023 18:41:10 GMT
RUN go version
# Wed, 06 Sep 2023 18:41:11 GMT
WORKDIR C:\go
```

-	Layers:
	-	`sha256:86fab75eb466cadf89d853682179b3b57eba9fe28c78041dd52bced81e18a627`  
		Last Modified: Tue, 08 Aug 2023 17:55:54 GMT  
		Size: 104.5 MB (104459386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:298e0f667b1d8252956bc07b8438d68801dd9eb4ebb7ad345fde0bed30609680`  
		Last Modified: Thu, 10 Aug 2023 01:03:59 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747b2e7b51c9236d6c6b9cf8e8129f1911ea80799d291f4a8b5957f6d27e6107`  
		Last Modified: Thu, 10 Aug 2023 01:03:59 GMT  
		Size: 1.1 KB (1114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8dc3f117353f426cabdbe4698ed536b1d14b31074ef744fc0e78ae81257c6da`  
		Last Modified: Thu, 10 Aug 2023 01:03:59 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56bd96136dc9cde131c7db62b4365b31f6f151da92ff74c6891c3cb17ffc436`  
		Last Modified: Thu, 10 Aug 2023 01:03:59 GMT  
		Size: 68.3 KB (68330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2a9ae8bec578f59df3b0eb0acdfd7fe97d2bf1d2a7a7b8880e037fd3fa58a1`  
		Last Modified: Thu, 10 Aug 2023 01:03:57 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc79c87f42e6aab5de77fff2e1dd9511c8f3e2f3edfb7e39f07b0c36019d423`  
		Last Modified: Wed, 06 Sep 2023 18:54:30 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dc1603bc2c10e8be6601182dfd72aa923d32d516d9fae3696e4b94f9333253`  
		Last Modified: Wed, 06 Sep 2023 18:54:47 GMT  
		Size: 69.1 MB (69063706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d5e2f06e8d1dac6b28cdc4c51802b3f4d67eeb915570a0eea2d714ab39c459`  
		Last Modified: Wed, 06 Sep 2023 18:54:30 GMT  
		Size: 77.9 KB (77919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5dd3fecd51f2a88a547558245ce4b9ef5bf01dca65dab9c2a6640ec2e8609c`  
		Last Modified: Wed, 06 Sep 2023 18:54:29 GMT  
		Size: 1.4 KB (1364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
