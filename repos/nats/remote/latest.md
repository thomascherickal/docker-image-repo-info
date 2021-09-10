## `nats:latest`

```console
$ docker pull nats@sha256:c812e8c75705b49bfc4694743b59428590372ff6689425c86ea3ddd682fd8c58
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2114; amd64

### `nats:latest` - linux; amd64

```console
$ docker pull nats@sha256:01dbe57fde6a40eecbd53edc6a418f3c9b1ddd85f03dd17e73ecef98a3b15318
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4546051 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80fcdf2bfe0f4a11267c9e8d06e5e52dce7dd9b41267e1a51d5e9df22c76bf9c`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:0b180121e1ef70970b020901a4b61990a8673ac9db99b94c348c5321333884ea in /nats-server 
# Fri, 10 Sep 2021 00:20:41 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:20:41 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:20:41 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:20:42 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:9cee557b7d3312d12996f8c4338bf9ea02657256657ef77d46510c729d9be195`  
		Last Modified: Fri, 10 Sep 2021 00:21:32 GMT  
		Size: 4.5 MB (4545577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb24b942a0d168497adac7ad3190098a6f8dfa34ad2ef37932150fbce9336c9a`  
		Last Modified: Fri, 10 Sep 2021 00:21:31 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v6

```console
$ docker pull nats@sha256:b21057f1f945b501d03cf3c5c2d530f7961e1a3198e00bb297b7f69a849cc0e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4210290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:865dcd8a77138e8339293c7089adeee440305e68331df5533186ea36b8132f84`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:50:15 GMT
COPY file:a60049eef2da0cbda1255e229e5e5c6377e3c3445b0cd16ce13a272139c7ce85 in /nats-server 
# Thu, 09 Sep 2021 23:50:16 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:50:17 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:50:17 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:50:18 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:b95232e9c9c31dfba5a6124fb74b4abc750a3fd6d5f89a13438a0b051430299e`  
		Last Modified: Thu, 09 Sep 2021 23:52:42 GMT  
		Size: 4.2 MB (4209813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c01128246ad2a36efed9386a5ed63a01f73f3f56e54d059834ac17a2f64a48`  
		Last Modified: Thu, 09 Sep 2021 23:52:38 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm variant v7

```console
$ docker pull nats@sha256:aafbb0b5e1b7412f9d0e71ddd6c3948c7080697882dd40ae20578b855ca40c1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4206272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:79f5a4fb5f9254997b2d7e573f24316740a167eb829bb23952ba05ff8304ddc1`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Fri, 10 Sep 2021 00:59:05 GMT
COPY file:7043dd814cd92048127f9905d58e9204d2968d9c03bbb7feba592c45a87e9963 in /nats-server 
# Fri, 10 Sep 2021 00:59:06 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Fri, 10 Sep 2021 00:59:06 GMT
EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:59:07 GMT
ENTRYPOINT ["/nats-server"]
# Fri, 10 Sep 2021 00:59:07 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:8ae70a7ddee0b3bc3819ff86ee31d3295a37b10282b7ee0d14d3dd3c8dcb16c7`  
		Last Modified: Fri, 10 Sep 2021 01:01:28 GMT  
		Size: 4.2 MB (4205795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbfbfa45875dc8bff20ba3a989407cf3ab8018f98f4277411dd068510c071c6`  
		Last Modified: Fri, 10 Sep 2021 01:01:25 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:24f192937e7bc371f7c2631055e49a51d489659d28f55b4fdf2eb5a19843a5ae
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4158958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cd8bb7e96599c9badd4424f86ef2d5f8561cfa0c4a4322057847c002da643a9`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 09 Sep 2021 23:40:25 GMT
COPY file:eda8ae8779fbfb7d34c95bc93fc8ce409cbd298cb302284f61ee4ebf6ac10b0e in /nats-server 
# Thu, 09 Sep 2021 23:40:26 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in /nats-server.conf 
# Thu, 09 Sep 2021 23:40:26 GMT
EXPOSE 4222 6222 8222
# Thu, 09 Sep 2021 23:40:26 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 09 Sep 2021 23:40:26 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0c0083faeb4bd1e89eefb7cbc2a5556eb056acaba6107a833c271a1ca7cd8633`  
		Last Modified: Thu, 09 Sep 2021 23:41:48 GMT  
		Size: 4.2 MB (4158481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4227e148c1053ae9735f2dcc2ab35b83566aab7b85aa3d50395ec15be4630e26`  
		Last Modified: Thu, 09 Sep 2021 23:41:47 GMT  
		Size: 477.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:latest` - windows version 10.0.17763.2114; amd64

```console
$ docker pull nats@sha256:da56a6dd1f9556f706d9086ed48947ac745a5b9dd1e3bc0d988581858828c23c
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107351558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:780da6fbe38cee622e2d2e69123219af601b417dada779a198cef0514370203e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 05 Aug 2021 19:15:20 GMT
RUN Apply image 1809-amd64
# Wed, 25 Aug 2021 16:07:56 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 10 Sep 2021 00:16:45 GMT
RUN cmd /S /C #(nop) COPY file:13fac1899b72f2f26df9bd8ce320e46a5f7736306d7abf82ea7d657c16444fb9 in C:\nats-server.exe 
# Fri, 10 Sep 2021 00:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 10 Sep 2021 00:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 10 Sep 2021 00:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:bc8517709e9cfff223cb034ff5be8fcbfa5409de286cdac9ae1b8878ebea6b84`  
		Size: 102.7 MB (102741177 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ae8616c17f5cca409a4b1289387e37dc532657ba2b52bb60713ff621acccd506`  
		Last Modified: Wed, 25 Aug 2021 16:11:20 GMT  
		Size: 1.0 KB (1022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55bd340c78387be49377457ea8e39875e7be9b3799bdac42ff35c749d67b3940`  
		Last Modified: Fri, 10 Sep 2021 00:20:25 GMT  
		Size: 4.6 MB (4604102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6782c003b15abdb2161dc360ffef0eeb967b34fc78186d8d6085aacfc85fa`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.8 KB (1777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf24d35e2c525beccaa7b227eda13492b401302f8ecc528e2a35118220e3f760`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71603cdad9bbdd669dd86cda1c010a6f91d1a58de21eac052a29279f77bd247f`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01477f3ed16729139c6a0a856de33336e03c4fb127df26c6e42b8157eaf1801b`  
		Last Modified: Fri, 10 Sep 2021 00:20:20 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
