## `nats:nanoserver`

```console
$ docker pull nats@sha256:3294eeea1a76a6480a18844a71ca4eba9c5dadf37f59b2bcb88c0f1231e96908
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `nats:nanoserver` - windows version 10.0.17763.1879; amd64

```console
$ docker pull nats@sha256:831f6df7bdb3be817528078e5b72613dabb70b92b7afd737d984ef3985110533
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105640788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0313ea64d6af8e0caf6349b7707e6afe60b3dd44538a3ee00e84141e548615e`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 08 Apr 2021 16:02:06 GMT
RUN Apply image 1809-amd64
# Wed, 14 Apr 2021 16:05:18 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Sat, 08 May 2021 01:16:08 GMT
RUN cmd /S /C #(nop) COPY file:535a754984bf10d9ddca3e2e88fba8d90931a64c61882f363dbd413ee28b3d6b in C:\nats-server.exe 
# Sat, 08 May 2021 01:16:09 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Sat, 08 May 2021 01:16:10 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Sat, 08 May 2021 01:16:11 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:ea84579f6cd5b58fe78732be37450bd188c8923de3a2062664f3992861449b5c`  
		Size: 101.3 MB (101340157 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f8d27bfefcaaa84a89f93945c61ccf0af9ad50b1405d9acfa30e9da5ba1fb2db`  
		Last Modified: Wed, 14 Apr 2021 16:10:39 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f09829f0860e906dc8a9d6c2c1e87e138239453a0be30fb920972b13e3606d`  
		Last Modified: Sat, 08 May 2021 01:20:33 GMT  
		Size: 4.3 MB (4294251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9528dc6daa3715f5a3085e1cdb49f94af36f2bda09aeaaf123872f17518c3081`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.8 KB (1789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ea30086cdda342e71659cbf1962edb5b19b66c43b27848cde55d6b64681154`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381d1211ca07f8b0ad6573f8e50245fdb903a1512b184bc6b3553bdd1eb89400`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95493f3ed9f68579900d31cf9dcdc01e2586365de53d6dd699961a2841c9ddb9`  
		Last Modified: Sat, 08 May 2021 01:20:31 GMT  
		Size: 1.1 KB (1096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
