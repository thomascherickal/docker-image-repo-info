## `mongo:4-nanoserver-1809`

```console
$ docker pull mongo@sha256:2c498a3d336b220dd86736b2e9178ad12c152f8076b0996fa9390844b557bb35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `mongo:4-nanoserver-1809` - windows version 10.0.17763.2237; amd64

```console
$ docker pull mongo@sha256:7fa0d1a228c3fd0e2b25aa1451b8f0454c2f0242680bedae5ee3d73f6c407aa2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.8 MB (335753878 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d827f9552c5970cc607d15d2002c27eb149095e1ab4b9d2c0fbca2013ba977f`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 12:53:34 GMT
SHELL [cmd /S /C]
# Thu, 14 Oct 2021 01:40:20 GMT
USER ContainerAdministrator
# Thu, 14 Oct 2021 01:40:33 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Thu, 14 Oct 2021 01:40:34 GMT
USER ContainerUser
# Thu, 14 Oct 2021 01:40:36 GMT
COPY multi:0196f9e96f60ad3e2b92fd0773f8d0fe3a8235e1eefbb9ef1a1f0d672e6a711c in C:\Windows\System32\ 
# Sat, 16 Oct 2021 00:20:19 GMT
ENV MONGO_VERSION=4.4.10
# Sat, 16 Oct 2021 00:20:45 GMT
COPY dir:38b7137ed0744364da7d2052947e6bc819b65de66682c9d7639e51a11bc90cfa in C:\mongodb 
# Sat, 16 Oct 2021 00:21:06 GMT
RUN mongo --version && mongod --version
# Sat, 16 Oct 2021 00:21:07 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 16 Oct 2021 00:21:08 GMT
EXPOSE 27017
# Sat, 16 Oct 2021 00:21:09 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:372f5dac265602794d3a4ddc20bd9845caf2acda0cec410704843c213a880da9`  
		Last Modified: Wed, 13 Oct 2021 13:29:46 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfae37dcc2021e3d10496776687736e4d2565f4b93492b8286aa9bd4a663324a`  
		Last Modified: Thu, 14 Oct 2021 02:19:23 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7b099be52eef9112df652bed33f01c48930744f308329472c54e09e00e77e79`  
		Last Modified: Thu, 14 Oct 2021 02:19:21 GMT  
		Size: 70.2 KB (70170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7102d479d05ed3a9336a5c5e5829142fb9489c43e80f3bcbcc9f22c71f1042f6`  
		Last Modified: Thu, 14 Oct 2021 02:19:21 GMT  
		Size: 1.1 KB (1059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455297daaaa79153573901a8796f77c2dd232e2709aeb8638e0b766abbc6875c`  
		Last Modified: Thu, 14 Oct 2021 02:19:21 GMT  
		Size: 274.0 KB (273992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d01bf7c69440ff15d97fe19ff0d34fb7c98411b8da1e51ff7d9568e54107e60d`  
		Last Modified: Sat, 16 Oct 2021 00:24:50 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48ec7df03feb64aba42ada5fe876ff4f58009c961957321882e094ab3cbf4a2`  
		Last Modified: Sat, 16 Oct 2021 00:25:30 GMT  
		Size: 232.7 MB (232655363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec1dcd69749ad197b57a38c3dc521853c11903cd7bad4a487c93f7737eafebf`  
		Last Modified: Sat, 16 Oct 2021 00:24:48 GMT  
		Size: 85.1 KB (85084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295806f382b17fa337da0c58b0246ba2eab432f0c53aebf21d707fa02eb4cc56`  
		Last Modified: Sat, 16 Oct 2021 00:24:48 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:084e2651e46b22af2877f9be72185f2331278a153d5e8365685f34cdbdb2b7f8`  
		Last Modified: Sat, 16 Oct 2021 00:24:48 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5027e5610590111e950eb1e8b1aa5657c1256a686804f760d16063993b89935`  
		Last Modified: Sat, 16 Oct 2021 00:24:48 GMT  
		Size: 1.1 KB (1092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
