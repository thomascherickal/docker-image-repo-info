## `hello-world:nanoserver`

```console
$ docker pull hello-world@sha256:8b23c064d218e2b4f91f687a334a904017e34dc573a30cde263c3ce2abc35376
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1366; amd64
	-	windows version 10.0.17763.3770; amd64

### `hello-world:nanoserver` - windows version 10.0.20348.1366; amd64

```console
$ docker pull hello-world@sha256:931f97f6715efc40b998b68159fccb663b6fdfdf4b323001205f762e9bab02f0
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122111197 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c8c5cf24eda0e5f6971a7b8c7db3a5da4bc5c3028277f35c63167171166c060`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Fri, 09 Dec 2022 09:19:21 GMT
RUN Apply image 10.0.20348.1366
# Wed, 14 Dec 2022 01:24:27 GMT
RUN cmd /S /C #(nop) COPY file:ac9f104fd739943f22886335a779468d86b20ac43fd3168171f6b23fc28882b9 in C: 
# Wed, 14 Dec 2022 01:24:27 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:70d3e1cc3b0ea172dcc93064fe6fb9f1f2c8fec6962c90e39991fe89a3c1ca03`  
		Last Modified: Wed, 14 Dec 2022 00:08:13 GMT  
		Size: 122.1 MB (122108200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b665be2399a25f3356be2bcd11b608906ffb3af6151a7ed1561c75b55f0da66`  
		Last Modified: Wed, 14 Dec 2022 01:24:52 GMT  
		Size: 1.9 KB (1896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c3ebd1894a76146640d44ca8f17a61a1922c6fd1453d54b99f7db832c2c2fa`  
		Last Modified: Wed, 14 Dec 2022 01:24:52 GMT  
		Size: 1.1 KB (1101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hello-world:nanoserver` - windows version 10.0.17763.3770; amd64

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
