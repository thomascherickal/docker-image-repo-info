## `mongo:4-nanoserver-ltsc2022`

```console
$ docker pull mongo@sha256:03cdfd360a853f8c1a1bab21f42a55e2fd2c0072d4ca31810594f79c06e9ed94
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1970; amd64

### `mongo:4-nanoserver-ltsc2022` - windows version 10.0.20348.1970; amd64

```console
$ docker pull mongo@sha256:5254625533a89fc75ab25d06b2ea8ebd12a71fc6fba7c92e26ae6d87049f3872
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **366.0 MB (366023795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a0003ede994ad5addb933745c5a1a8c9dac2e54f18435ac7be36a183cc2e27b`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Fri, 01 Sep 2023 00:20:14 GMT
RUN Apply image 10.0.20348.1970
# Wed, 13 Sep 2023 01:45:13 GMT
SHELL [cmd /S /C]
# Wed, 13 Sep 2023 04:00:25 GMT
USER ContainerAdministrator
# Wed, 13 Sep 2023 04:00:30 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 13 Sep 2023 04:00:31 GMT
USER ContainerUser
# Wed, 13 Sep 2023 04:21:27 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Wed, 13 Sep 2023 04:32:12 GMT
ENV MONGO_VERSION=4.4.24
# Wed, 13 Sep 2023 04:32:32 GMT
COPY dir:1066042ae200f96ac2fccaeb2deab7c0e3f03606d0c552a57bf93bf4149d79fb in C:\mongodb 
# Wed, 13 Sep 2023 04:32:41 GMT
RUN mongo --version && mongod --version
# Wed, 13 Sep 2023 04:32:42 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 13 Sep 2023 04:32:43 GMT
EXPOSE 27017
# Wed, 13 Sep 2023 04:32:43 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:8f8cef0759210af9d01a2fb45d79956a2db738bbd3734b7244b17e14ad945cab`  
		Last Modified: Tue, 12 Sep 2023 18:47:39 GMT  
		Size: 120.6 MB (120567584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c795bb9d48e9fa247e549604525fcb2599507cf1008aa1df12036f428ea236d`  
		Last Modified: Wed, 13 Sep 2023 02:18:07 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4d4f6211677cf82e6ed0d87f108ca902b6953cac7069b26a23966ebb167924`  
		Last Modified: Wed, 13 Sep 2023 04:38:18 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:409b27824df1096550781d8d27fdafeb1abf5437c93f4d7bce18fdab09d1a67c`  
		Last Modified: Wed, 13 Sep 2023 04:38:16 GMT  
		Size: 79.5 KB (79488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01ed47b78f8c73c7cb1a91613a90350ec6f08cbad9f792825e0a51f4f144fd0`  
		Last Modified: Wed, 13 Sep 2023 04:38:16 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d1c7ce100358fa46d16a3327a47a66e4351aee22769f947d1afd110e118b21`  
		Last Modified: Wed, 13 Sep 2023 04:54:11 GMT  
		Size: 263.4 KB (263377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9bdcace8e44136f7653858c204b4dbf9a7f2494c3ec19be5f22ed3680a058b1`  
		Last Modified: Wed, 13 Sep 2023 05:02:07 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b41e873eb0f45bb812891cf70177a6050313ec99d66bf07215a33ccbb2f741`  
		Last Modified: Wed, 13 Sep 2023 05:02:42 GMT  
		Size: 245.0 MB (245044519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1376da5c8f64251941ac0b1a0342be122c708fbaae92af1b86b9d6e08cc4cd0`  
		Last Modified: Wed, 13 Sep 2023 05:02:05 GMT  
		Size: 60.7 KB (60746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bd6dea0626e4f1f94f974f2f7b8cdfdcac31e0feb7b0049944f3446d1f13334`  
		Last Modified: Wed, 13 Sep 2023 05:02:05 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149af6d46f29857bd888060cade6c53c5b2babfcd027b8886d1df366241c3076`  
		Last Modified: Wed, 13 Sep 2023 05:02:05 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feecd163d985e6f24523c9a909d2f440ae2b624edf7aa8bc850913bce22588fa`  
		Last Modified: Wed, 13 Sep 2023 05:02:05 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
