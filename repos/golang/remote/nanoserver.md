## `golang:nanoserver`

```console
$ docker pull golang@sha256:714df6b11323bebc55e36405ea9152f9ebaf314d91836ec8314646ef54bfcf5f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1040; amd64

### `golang:nanoserver` - windows version 10.0.17763.1040; amd64

```console
$ docker pull golang@sha256:673a04bc637a1374037c5a88e2ecae44677ce7280655a368d3273e08194d4886
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234145578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30807218151688747ca9bd7bcfcfa4cec67ece9e47f5c3f027496f5cb29c3341`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Sun, 16 Feb 2020 01:25:57 GMT
RUN Apply image 1809-amd64
# Thu, 20 Feb 2020 09:32:26 GMT
SHELL [cmd /S /C]
# Thu, 20 Feb 2020 09:32:27 GMT
ENV GOPATH=C:\gopath
# Thu, 20 Feb 2020 09:32:28 GMT
USER ContainerAdministrator
# Thu, 20 Feb 2020 09:32:43 GMT
RUN setx /m PATH "%GOPATH%\bin;C:\go\bin;%PATH%"
# Thu, 20 Feb 2020 09:32:44 GMT
USER ContainerUser
# Wed, 26 Feb 2020 00:38:19 GMT
ENV GOLANG_VERSION=1.14
# Wed, 26 Feb 2020 00:43:35 GMT
COPY dir:d9f92e2bb48fc91c25fbd35b77ed7dfa18307cbb29a039e6f056274a3e4184df in C:\go 
# Wed, 26 Feb 2020 00:43:53 GMT
RUN go version
# Wed, 26 Feb 2020 00:43:54 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:a35da61c356213336e646756218539950461ff2bf096badf307a23add6e70053`  
		Size: 101.1 MB (101145811 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1f92100f2e1b3af3a5a0d84762c4044d22c99f98202c80fb4292e4f45f83d8c4`  
		Last Modified: Thu, 20 Feb 2020 10:21:07 GMT  
		Size: 948.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5f0b59f3e59e9d0a21f61515b9db1772feeb1261fa24dfb1bef6fb437455de`  
		Last Modified: Thu, 20 Feb 2020 10:21:06 GMT  
		Size: 925.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ae466e51b0e2a397016e915135c9a3a9eabca5aec1bf58b75f629149fa8ebb`  
		Last Modified: Thu, 20 Feb 2020 10:21:06 GMT  
		Size: 944.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95115058bc58d97985100f2ff9a9fdb06d410d2a165b2511e905c6cbb312a729`  
		Last Modified: Thu, 20 Feb 2020 10:21:06 GMT  
		Size: 63.3 KB (63336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d6d28ec71964f78de5b64d55be0959e13875b24ead023084654b49d1fbbf754`  
		Last Modified: Thu, 20 Feb 2020 10:21:04 GMT  
		Size: 922.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a1e196039ca44e2e3a7708814528abda6a8a21e695ef6e35a62ff9d7dea137`  
		Last Modified: Wed, 26 Feb 2020 00:49:50 GMT  
		Size: 916.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbd2a6b089b3935f460c33e772d3714628eae5aed520bf460499f1ec88bc629`  
		Last Modified: Wed, 26 Feb 2020 00:51:36 GMT  
		Size: 132.9 MB (132864434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd47ac9aaeef51ecbb366e03ab784c578c72fb6dc3caacdeec007b03ff30088`  
		Last Modified: Wed, 26 Feb 2020 00:49:50 GMT  
		Size: 66.2 KB (66186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1313e7c8806b7c80df4fbddb3870cba7338058276d7e8fbfe6d9d429b2a688e7`  
		Last Modified: Wed, 26 Feb 2020 00:49:50 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
