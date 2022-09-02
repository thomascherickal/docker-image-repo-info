## `buildpack-deps:jammy-curl`

```console
$ docker pull buildpack-deps@sha256:323aa4146bcd5317e5841a7be255565d063a92b92316109e85688fa2094f763f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:jammy-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8b8f7edeac757b1a514d89c5f6e4082b9f64b1aeb87eeaa31da58dbe9e424ff6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.8 MB (37791656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32d70c81850c25c6f5bf209fbcc9e0b2732e5456ebcaf907d4a139b4e73eb4e7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:35 GMT
ADD file:a7268f82a86219801950401c224cabbdd83ef510a7c71396b25f70c2639ae4fa in / 
# Thu, 01 Sep 2022 23:46:35 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:27:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:2b55860d4c667a7200a0cb279aec26777df61e5d3530388f223ce7859d566e7a`  
		Last Modified: Tue, 16 Aug 2022 03:03:54 GMT  
		Size: 30.4 MB (30426706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728cfcfa2f7739d87ae3efda60d01680593fcb2b55fdb5840721012c19335b9a`  
		Last Modified: Fri, 02 Sep 2022 02:38:25 GMT  
		Size: 3.8 MB (3804276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09eda6154af3733cdc766a287039ebbd0d78265b3a7c64ed165045c8849ba1ce`  
		Last Modified: Fri, 02 Sep 2022 02:38:25 GMT  
		Size: 3.6 MB (3560674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:dd3bd02cb06b00a6b0e05290d62dfc04f462a233d96b82fec29f39be0585b5cb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34302694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0783d26fd063b045a6a6d1ad7484a25a49f96420d15956b66d9c6a1fdd8f06a0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:40:56 GMT
ADD file:1bec4ea562c9a42add30f5e3626edc93bdfc0271cbd208a4447842fa31b5c114 in / 
# Tue, 02 Aug 2022 01:40:56 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:58:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:58:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f1a5cf9a21e485b0a676c22ced0e80a140055b3ef0d7573caf5be408a10ddb04`  
		Last Modified: Tue, 02 Aug 2022 01:43:32 GMT  
		Size: 27.0 MB (27017015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7f5e1bf5a769b4cdcff0e4f7232bd3bf5f7d07c3f23ff030f74cf0abd24053`  
		Last Modified: Tue, 02 Aug 2022 02:16:37 GMT  
		Size: 3.6 MB (3572129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3fd3be308fda95edf60931006bd4d3432d41d1a26e5942a75d3f6e89282df28`  
		Last Modified: Tue, 02 Aug 2022 02:16:36 GMT  
		Size: 3.7 MB (3713550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:46fc6e142336fbe53686a9b32ce2588ef1d88236df5f1d28f8a010c9a37af054
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35495544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0b8f89e44d753f137abf471fdef52e03ea28cb68bf54efeb4813576f3fe06fb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:18:59 GMT
ADD file:3db67543ea64bf6723921d19cc5d0483db5c6658fc95834d8b2b5ed48a4cbacd in / 
# Tue, 02 Aug 2022 01:18:59 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:35:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:35:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:4a3049d340b7d3651a954fd25a32c42feb1086889d6287e2f15468aef865c5c4`  
		Last Modified: Tue, 02 Aug 2022 01:20:49 GMT  
		Size: 28.4 MB (28381155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6de042cb869a25eebdf68de514b4450f82c38b9cec853a790e0bc12272588d`  
		Last Modified: Tue, 02 Aug 2022 01:50:49 GMT  
		Size: 3.8 MB (3793545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efd2a11a62cb05975c115b200176aa1783cf879e07bb4ee462cf161275ec087`  
		Last Modified: Tue, 02 Aug 2022 01:50:49 GMT  
		Size: 3.3 MB (3320844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f90616501e56c0a29c314b116b5b9ce5f53aa9e7a0d42ae9b5c753c919d3e39c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44241852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1635ae01ceaf220af350d6734387396e2064e26580b565afcc09d0e6bfcc5659`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:31:12 GMT
ADD file:b6916c28c03568df4c2efc3da91ea6320f639cdbd2fa3f6741fcea7acad4fd5f in / 
# Tue, 02 Aug 2022 01:31:14 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:53:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:53:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:6f8c2fc0a4f976c1c0bd1c0e14022b3ed8b7c83cdb247c83016052c3678aaf28`  
		Last Modified: Tue, 02 Aug 2022 01:33:53 GMT  
		Size: 35.7 MB (35718004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc064b2f92ee9486c5aff9b01b6c4e03b1dabb079057e9522378da6a679d656f`  
		Last Modified: Tue, 02 Aug 2022 03:23:01 GMT  
		Size: 4.3 MB (4290202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85366274834fa0723d3cae9a97e7aa88f9e031aa2c26e64e8d90d3650c2e978f`  
		Last Modified: Tue, 02 Aug 2022 03:23:01 GMT  
		Size: 4.2 MB (4233646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:37a6e4bfff70a1d2f2343ec0bc7c5b663942e36f797247df635b8586266c5ce8
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.1 MB (35138019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:243eb39738059da136ec1fc770b105776ec3d66b623f2e08cb79cfb2b16709fc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 00:11:51 GMT
ADD file:8cff03722326c5e90e26ae259bde7ddd223c466edfd0d1cd6335b7b550f8156c in / 
# Fri, 02 Sep 2022 00:11:52 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 01:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:03:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:f04a8971a8d913388890f40190f4d3935404b38efd860b235cf5d4de20959061`  
		Last Modified: Fri, 02 Sep 2022 00:29:20 GMT  
		Size: 27.7 MB (27744005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c893dcd3d9a55418817428155b89e044a2ebfddfa13d6945d70f0e2830099015`  
		Last Modified: Fri, 02 Sep 2022 01:49:29 GMT  
		Size: 3.6 MB (3615909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8351e367bac61d27e9f493ab2fdd756510203f5c595c3c81d6b96d2ac3214ca`  
		Last Modified: Fri, 02 Sep 2022 01:49:27 GMT  
		Size: 3.8 MB (3778105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:6a7bc5b2496502a65bad30f7cb0b243ced4eed84af1897e94b98cbc971af9aa6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35924452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59742e1d75395c6a6342d0534baf73e19ecec72302e69af41dbd4cf5ac64fe0c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:25 GMT
ADD file:aabc057fd7b1b1f9b4b729222b6dc90e98f846a65bfee1ee57cc899b6cee5a10 in / 
# Fri, 02 Sep 2022 01:03:28 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:06:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:07:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
```

-	Layers:
	-	`sha256:a32e6a15a6635185097921b9d08997d505b6b6500b6c142ad8e718d87c45ffad`  
		Last Modified: Fri, 02 Sep 2022 01:05:01 GMT  
		Size: 28.6 MB (28643161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba21c1eef45ab363d5dcc84511ca01cdbbe1e6dfdf54dcd8b108e256251e6e5`  
		Last Modified: Fri, 02 Sep 2022 02:16:20 GMT  
		Size: 3.8 MB (3809432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b26595dd670dde31a9dd83588e0dd3408a0d7f51791314f04652f5117a00332`  
		Last Modified: Fri, 02 Sep 2022 02:16:20 GMT  
		Size: 3.5 MB (3471859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
