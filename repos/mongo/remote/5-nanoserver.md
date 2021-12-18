## `mongo:5-nanoserver`

```console
$ docker pull mongo@sha256:cafb9d048b042e690323e436b0499f117009a6851cffe686a596f5bf92fcf729
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.405; amd64
	-	windows version 10.0.17763.2366; amd64

### `mongo:5-nanoserver` - windows version 10.0.20348.405; amd64

```console
$ docker pull mongo@sha256:625accfd8256290936520811c13e2f94d0637a4c3e5f73b3f621f9c0aa42ddd8
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **411.6 MB (411591061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:36ebb353bbaedc8c99ba448a50edad3c682e776e7cbca4d7872b54c1715a0d11`
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
# Sat, 18 Dec 2021 08:15:38 GMT
ENV MONGO_VERSION=5.0.5
# Sat, 18 Dec 2021 08:16:11 GMT
COPY dir:97e0851993a8443e809dbfb982fa612becf2ad4c3b07d76c242613492af3987d in C:\mongodb 
# Sat, 18 Dec 2021 08:16:24 GMT
RUN mongo --version && mongod --version
# Sat, 18 Dec 2021 08:16:25 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 18 Dec 2021 08:16:26 GMT
EXPOSE 27017
# Sat, 18 Dec 2021 08:16:27 GMT
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
	-	`sha256:b82a6e2ad4dd68daf4717636f65b3bcd884f02f6b5eed91520a59f30672f9dd3`  
		Last Modified: Sat, 18 Dec 2021 09:14:49 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046d1dad0a652fdb614497069d16eae0b50744e24a9e589cc63f5d234c4a217e`  
		Last Modified: Sat, 18 Dec 2021 09:15:43 GMT  
		Size: 293.9 MB (293936078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b42befe8bb6d432e5094981fa69e99c50b435884129485ed3f84502104321f1`  
		Last Modified: Sat, 18 Dec 2021 09:14:47 GMT  
		Size: 61.5 KB (61523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c3373a3c76b3cdd46ab16445c8096dea099880f3b3c8aee1fbae5a79c4bc78c`  
		Last Modified: Sat, 18 Dec 2021 09:14:47 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a9c08a72673730c56e3d71b248fe6ae88fad77ae50ba7244a66f873f75bd42`  
		Last Modified: Sat, 18 Dec 2021 09:14:47 GMT  
		Size: 1.2 KB (1167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171bdf96b28c82ceeba9c9a0736c1e44adfa34ea80ee8c63c6d964bf49a71a65`  
		Last Modified: Sat, 18 Dec 2021 09:14:47 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mongo:5-nanoserver` - windows version 10.0.17763.2366; amd64

```console
$ docker pull mongo@sha256:1acde3edf979a2fc5b1e4f18fc9abac01212f7a67bea841e62f1e3fa26716c08
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **397.3 MB (397253310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb88604eb40c3a7c30205124125f1fecb2d91d62598bb32ed0aa7466bf71bd9a`
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
# Sat, 18 Dec 2021 08:16:50 GMT
ENV MONGO_VERSION=5.0.5
# Sat, 18 Dec 2021 08:17:21 GMT
COPY dir:97e0851993a8443e809dbfb982fa612becf2ad4c3b07d76c242613492af3987d in C:\mongodb 
# Sat, 18 Dec 2021 08:17:34 GMT
RUN mongo --version && mongod --version
# Sat, 18 Dec 2021 08:17:34 GMT
VOLUME [C:\data\db C:\data\configdb]
# Sat, 18 Dec 2021 08:17:35 GMT
EXPOSE 27017
# Sat, 18 Dec 2021 08:17:36 GMT
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
	-	`sha256:4dbef671ddc89b3065337fe53a513488717348b13a8289635891445e9f2b06d5`  
		Last Modified: Sat, 18 Dec 2021 09:16:01 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28202325cffa4c9efc5b58aba13b3744688c1f541ed0e494692474879ece11e1`  
		Last Modified: Sat, 18 Dec 2021 09:16:50 GMT  
		Size: 293.9 MB (293935952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b581c9c55af293079db450ae4c695b14070f627b38d5e8eda5a55181bb719e`  
		Last Modified: Sat, 18 Dec 2021 09:15:59 GMT  
		Size: 56.2 KB (56174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3278705964f3225d56e256c4a6fc6cab7af4da777915328e8d2f14ed1f63322a`  
		Last Modified: Sat, 18 Dec 2021 09:15:59 GMT  
		Size: 1.2 KB (1160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c358b5fe64605a8ac6b70f9a82de9079261d15fda8b7f80d93b5825f5e6c88c`  
		Last Modified: Sat, 18 Dec 2021 09:15:59 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5269ea8fed398510bb7f6c967a5f6f34de44395a98be6b3f6aab91d5d232892`  
		Last Modified: Sat, 18 Dec 2021 09:15:59 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
