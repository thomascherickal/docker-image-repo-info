## `mongo:4-nanoserver`

```console
$ docker pull mongo@sha256:461f5e95a34ea35c7904ea786d79b219bc3af8211217b921615b7ad2af4128c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.405; amd64
	-	windows version 10.0.17763.2366; amd64

### `mongo:4-nanoserver` - windows version 10.0.20348.405; amd64

```console
$ docker pull mongo@sha256:58561cde05b6251fbdead64f631d54a70987733dfaaf84f1d63ca394df9f07ef
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **350.3 MB (350310431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65b2694833fc2161db93b473cf582498eb1373c176e0983c397aca71d95ab31f`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Wed, 08 Dec 2021 01:24:33 GMT
RUN Apply image ltsc2022-amd64
# Sat, 18 Dec 2021 00:29:51 GMT
SHELL [cmd /S /C]
# Sat, 18 Dec 2021 08:15:19 GMT
USER ContainerAdministrator
# Sat, 18 Dec 2021 08:15:35 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Sat, 18 Dec 2021 08:15:36 GMT
USER ContainerUser
# Sat, 18 Dec 2021 08:15:37 GMT
COPY multi:0196f9e96f60ad3e2b92fd0773f8d0fe3a8235e1eefbb9ef1a1f0d672e6a711c in C:\Windows\System32\ 
# Sat, 18 Dec 2021 08:33:28 GMT
ENV MONGO_VERSION=4.4.10
# Sat, 18 Dec 2021 08:33:52 GMT
COPY dir:38b7137ed0744364da7d2052947e6bc819b65de66682c9d7639e51a11bc90cfa in C:\mongodb 
# Sat, 18 Dec 2021 08:34:24 GMT
RUN mongo --version && mongod --version
# Sat, 18 Dec 2021 08:34:25 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 18 Dec 2021 08:34:26 GMT
EXPOSE 27017
# Sat, 18 Dec 2021 08:34:26 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:11961e4f2e13a442b572d4bc37edfe94ad6d8c2ed378f0dcae8b880959c4b538`  
		Size: 117.2 MB (117225770 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5f7005dc509dad3c53e79bd72ff76e4dda4a38b2eee2264ceb864eaa233dab99`  
		Last Modified: Sat, 18 Dec 2021 01:23:16 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a67bd3e0ca03c1f7f2c9eeca331b2bbd9ccb82a21c268583c08f3abb150c7b`  
		Last Modified: Sat, 18 Dec 2021 09:14:52 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85c2b4d3226c6c176627e2fd5c006c51b6f366800df3421719cdadac481522f`  
		Last Modified: Sat, 18 Dec 2021 09:14:52 GMT  
		Size: 85.5 KB (85503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91704e831785bce2a5c9b408b573b3d078bb99bcb996e7bc7dd7116a785cff59`  
		Last Modified: Sat, 18 Dec 2021 09:14:50 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:639aa194d1e3e2583ce54164c43194229bae1094723cabb5aa1bdf24c198d231`  
		Last Modified: Sat, 18 Dec 2021 09:14:50 GMT  
		Size: 274.1 KB (274104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d496f0ebac94247c5b93d77da479d53135a63fa3fa24ef6e5e8cdcd6112c49`  
		Last Modified: Sat, 18 Dec 2021 09:42:18 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162f2058b7d3e93908fc6aa6d66307a00ccafb58df0bf68d5e6573c1c37a5610`  
		Last Modified: Sat, 18 Dec 2021 09:43:01 GMT  
		Size: 232.7 MB (232655430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df7122bdce4cda3efac1ada5b909a4409d7f2e1a379e6e453d6f61711d93a2ff`  
		Last Modified: Sat, 18 Dec 2021 09:42:16 GMT  
		Size: 61.5 KB (61494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76575a6aab95b74f24b37ebb0b294783bd95f72a49861ccb0f1c4211272bc2e1`  
		Last Modified: Sat, 18 Dec 2021 09:42:16 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87d2d484c0ece33e19f8f6e15c3aa76412df9c9ff8ad373734ab029b0627b60`  
		Last Modified: Sat, 18 Dec 2021 09:42:16 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a56abcde1ec30ab07d59caaa5f87bbb6f75d33f2904fa72267853942520484f`  
		Last Modified: Sat, 18 Dec 2021 09:42:16 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:4-nanoserver` - windows version 10.0.17763.2366; amd64

```console
$ docker pull mongo@sha256:ca8d70a9075d5ed658ffd04768bc23af1ebe206d8bb49522ac5371bcdc8f4e44
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.0 MB (335960307 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c5b95a186be291ff0f55d2cbfeb50d564e023b82cab0155e9fa329b9b6337d7`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Tue, 07 Dec 2021 04:37:11 GMT
RUN Apply image 1809-amd64
# Sat, 18 Dec 2021 00:33:50 GMT
SHELL [cmd /S /C]
# Sat, 18 Dec 2021 08:16:34 GMT
USER ContainerAdministrator
# Sat, 18 Dec 2021 08:16:47 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Sat, 18 Dec 2021 08:16:47 GMT
USER ContainerUser
# Sat, 18 Dec 2021 08:16:49 GMT
COPY multi:0196f9e96f60ad3e2b92fd0773f8d0fe3a8235e1eefbb9ef1a1f0d672e6a711c in C:\Windows\System32\ 
# Sat, 18 Dec 2021 08:34:41 GMT
ENV MONGO_VERSION=4.4.10
# Sat, 18 Dec 2021 08:35:07 GMT
COPY dir:38b7137ed0744364da7d2052947e6bc819b65de66682c9d7639e51a11bc90cfa in C:\mongodb 
# Sat, 18 Dec 2021 08:35:52 GMT
RUN mongo --version && mongod --version
# Sat, 18 Dec 2021 08:35:53 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 18 Dec 2021 08:35:54 GMT
EXPOSE 27017
# Sat, 18 Dec 2021 08:35:55 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:034b2f457cdf6a0d3f7024523d40fd6eeb8568e6c76d9fa56f4053fcf3a21d63`  
		Size: 102.9 MB (102904001 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dac80fcd8aee90ad8a9145e0685b7c90d701307507ff32ffed6c86abc09c0f7a`  
		Last Modified: Sat, 18 Dec 2021 01:24:07 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ecafa7fdca0a8d9bbb541c6c503af8429d2b056d7ef10720fb63ee2ccd99df`  
		Last Modified: Sat, 18 Dec 2021 09:16:03 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1d19af80dba399d3a20765b575762747430f0cf5cc5d89e269a3a453340d26`  
		Last Modified: Sat, 18 Dec 2021 09:16:02 GMT  
		Size: 75.0 KB (75014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6472f76c36dc4c357b0583bd0592fee8c1568824ca166f1c8dbd66ad4c3cafe9`  
		Last Modified: Sat, 18 Dec 2021 09:16:01 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801875e2c17752512e14d76ddbedcd4b5b966101d38861c26a2567cc67f5282f`  
		Last Modified: Sat, 18 Dec 2021 09:16:01 GMT  
		Size: 274.1 KB (274067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b6e8c449c5fd0d3fd413a4e606aa94e4c0b45c4471a918eb31d244d1307c247`  
		Last Modified: Sat, 18 Dec 2021 09:43:16 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e5e57a8d79d545b4ad25d02feac910a6e744da4be73f91e9d259d0399e61f47`  
		Last Modified: Sat, 18 Dec 2021 09:43:58 GMT  
		Size: 232.7 MB (232656668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ef2b6b6e7425df3b2846425b310a233058e31842f1d4694f682514ec59efe13`  
		Last Modified: Sat, 18 Dec 2021 09:43:14 GMT  
		Size: 42.5 KB (42545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e6f2c9f06130c89869fd0280f2912e17e92a7781a6f4819fd247fdc3fb1540`  
		Last Modified: Sat, 18 Dec 2021 09:43:14 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc3372a6aa3b9e070fcedf060f7deeceee46c17a26fd6160d5421fcead2b9fb0`  
		Last Modified: Sat, 18 Dec 2021 09:43:14 GMT  
		Size: 1.2 KB (1157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:935d3dcbf335a5411685a540dc2cc8b60854aaa4b784def86b83aba6f323c07d`  
		Last Modified: Sat, 18 Dec 2021 09:43:15 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
