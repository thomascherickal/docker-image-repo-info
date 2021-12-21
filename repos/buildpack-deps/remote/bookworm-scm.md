## `buildpack-deps:bookworm-scm`

```console
$ docker pull buildpack-deps@sha256:069cdc6bbc7b0ffe7c5f627fe29b9f7bb029395b2c4ca7a8aa0fe326d0b7c219
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bookworm-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:3c3a1765c3e48bf5c4f7264812e232f025474870ab4cfd73c7d5f616beeac221
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.5 MB (128502529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a91bea1b1534aba933cb992f9fcee870891f5f759499f215fa31047e20c590e7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:09 GMT
ADD file:15e5b0a35c4fc7a5ae0bf08f713bde738d2cfb06a30b8bd5780fabafb91d934c in / 
# Tue, 21 Dec 2021 01:22:10 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:50:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:50:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 01:50:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9aa4f47c6909274e4d7f0b2429a7ad24598b19c01da78245a16a3176f9acf847`  
		Last Modified: Tue, 21 Dec 2021 01:26:44 GMT  
		Size: 55.6 MB (55598801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f71e2132b1cfc0df72e7252fbbc759f38ec76718cbb194e3f3abae59f6c6f7`  
		Last Modified: Tue, 21 Dec 2021 02:00:06 GMT  
		Size: 5.3 MB (5282859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76f2c25fefbc6f35b9aa1d2da6608ac2eca9de0a624ef3624ea94b11c7ed3db4`  
		Last Modified: Tue, 21 Dec 2021 02:00:06 GMT  
		Size: 10.9 MB (10904095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5817e8417410ab0f6ecb2677bde006e866e271aa33c4338c69a38955bc4b585a`  
		Last Modified: Tue, 21 Dec 2021 02:00:27 GMT  
		Size: 56.7 MB (56716774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6054246b532a8ed5a529251699f4b72e00929b657711f1847428fcb8f32b70c9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122837263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c3aa7ddb9e25df7df216f8a37a08fb13da9791eb046b933f65f8fc1e143dbd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 02:49:00 GMT
ADD file:565dc0a92c6ce86500c032d7c7e8112f62771ff3bac3aa84192e8309ae7acbba in / 
# Thu, 02 Dec 2021 02:49:03 GMT
CMD ["bash"]
# Fri, 10 Dec 2021 21:49:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 10 Dec 2021 21:49:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 10 Dec 2021 21:50:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:92dd04f71649984a91d8241840b2fa0a06cee72bebcd6503ece93ae1b5f47d07`  
		Last Modified: Thu, 02 Dec 2021 03:07:38 GMT  
		Size: 53.0 MB (53031153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034d98e044e9e53481f8d4d8abf3a1c951af6e2e0302f2d5c7b0bafe2d4ef536`  
		Last Modified: Fri, 10 Dec 2021 21:58:02 GMT  
		Size: 5.2 MB (5181891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c07dfbba8655504d3ed9b02abdf2cb4d87d6795189ed0afd4f34e9f46363bebf`  
		Last Modified: Fri, 10 Dec 2021 21:58:04 GMT  
		Size: 10.6 MB (10610919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513592010d54422089f4ecc08fde13540373b391c1a925acf5521999a5efd10e`  
		Last Modified: Fri, 10 Dec 2021 21:58:54 GMT  
		Size: 54.0 MB (54013300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0231b7a4b81ac92a6b5c7dc57477b4f78ce0230e825f67f0c272bb8ba1896701
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.9 MB (117852377 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:686b0e05328de0c16286f8b466efe0013a7c88a58ffbed4ba40a4baacf40a060`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 09:03:39 GMT
ADD file:bd5233b326b625660d820fa962832e6c5413ff9a56f64a6f072b9a9adfc545b2 in / 
# Thu, 02 Dec 2021 09:03:40 GMT
CMD ["bash"]
# Fri, 10 Dec 2021 21:58:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 10 Dec 2021 21:58:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 10 Dec 2021 21:59:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4dcb906f06af542b010e092a9a4d4ad8ccb110debf57beb0d4ded9baa51b82a1`  
		Last Modified: Thu, 02 Dec 2021 09:18:59 GMT  
		Size: 50.7 MB (50667986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6290470e339a2322159fc965896cd31eecd849410e2d52a8d8ecfd35f27f39`  
		Last Modified: Fri, 10 Dec 2021 22:10:56 GMT  
		Size: 5.0 MB (5041382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dffd92cf9cc4dbaae187824ff4063b4fb6ee16274347a41c15b4c1609885dcfd`  
		Last Modified: Fri, 10 Dec 2021 22:10:58 GMT  
		Size: 10.3 MB (10253459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c9c9fb9112e13c18c8c06ca220eb290b49016d39cfe010810870e8b8dc90af`  
		Last Modified: Fri, 10 Dec 2021 22:11:45 GMT  
		Size: 51.9 MB (51889550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:e35bcd0e9c3d722112b78b3e835c14be98c719bca231351b658344252ece7ca2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127303943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f324c1af26c172a528d4cae75a2ee4853071d00614623743df39bb3257545ef`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:41:45 GMT
ADD file:c64482c2e0b0935b000b024e468499d2586b78ca5c64b035ded7ce33f1dabe14 in / 
# Tue, 21 Dec 2021 01:41:45 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:10:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:10:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:10:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be902f523b4c4ddf53ea157e340cd7ce836ec2a0952d6f18602467352524e312`  
		Last Modified: Tue, 21 Dec 2021 01:47:42 GMT  
		Size: 54.6 MB (54598073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ae3b1dd188183d78f548c40b842d6abda988dc1e02042a8d2fbba1292db6225`  
		Last Modified: Tue, 21 Dec 2021 02:21:21 GMT  
		Size: 5.3 MB (5271381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d762390d417c63f26301db70b2fc0b6cbfb2a625b710902a4efa39a4fbe7eeac`  
		Last Modified: Tue, 21 Dec 2021 02:21:21 GMT  
		Size: 10.7 MB (10679800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a737f25eeff639378bcc151ec6663db78937cc6769ac1822011ac7d273f3638`  
		Last Modified: Tue, 21 Dec 2021 02:21:41 GMT  
		Size: 56.8 MB (56754689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:12d01844245eefebce5291c5506d40dfd261f365ee44d58b1f8b1853d19454e2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.5 MB (131491117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:905c2c5c61940a09c5dccd7b60d1249a4e82912670e393010349e445eb99b918`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:39:06 GMT
ADD file:f5394800b665e61b6f319d6dffbccd66c1172d4e9fd1db6ba962ef5aa177c353 in / 
# Tue, 21 Dec 2021 01:39:06 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:11:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:11:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:11:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:75388d3fd5f848339be12f5cd41cdf79effd086f4656396bfbac934b7f1f715c`  
		Last Modified: Tue, 21 Dec 2021 01:47:16 GMT  
		Size: 56.7 MB (56658883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de7e33a377d91eac773d98f83f6ca3f85f496a95ef1607a2f5af89fb4471391`  
		Last Modified: Tue, 21 Dec 2021 02:24:06 GMT  
		Size: 5.4 MB (5414374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4180045f386d2f79d4770aa88797a1fda448758575d57afc6ea4e781dc548b5c`  
		Last Modified: Tue, 21 Dec 2021 02:24:07 GMT  
		Size: 11.3 MB (11285476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13c98f4c5e2e21a446971fb90d2f11dea323e9e79c68d747e0a9e0a487d9a02b`  
		Last Modified: Tue, 21 Dec 2021 02:24:34 GMT  
		Size: 58.1 MB (58132384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6e9ecb1eae6ba0e275802cf2a88e24e944898182f34bea7985650587e622dce4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.6 MB (125568426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd4c2211de0e2611d11e8dd148d155cc777fae0f0c16b4994060d7f12ce936fd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 03:07:51 GMT
ADD file:2b78b392bcc6daef3d9c93dcae4adf8b84cac89c57ed08bd43854d23774078d6 in / 
# Thu, 02 Dec 2021 03:07:52 GMT
CMD ["bash"]
# Fri, 10 Dec 2021 22:07:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 10 Dec 2021 22:08:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 10 Dec 2021 22:09:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8c4a35c3e932252ccb2418c1bc14531f11d21f13ba131d0a52cd9cb690dc9623`  
		Last Modified: Thu, 02 Dec 2021 03:15:53 GMT  
		Size: 54.3 MB (54269592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5382fc82d142248068645a004ecdcba9b86008e8e6d072fb2a8b85524a38c87c`  
		Last Modified: Fri, 10 Dec 2021 22:12:49 GMT  
		Size: 5.2 MB (5239618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715d5f987669cd4335e12d30a8b21fb2532368af6d0867a4749dc32ef5e0350f`  
		Last Modified: Fri, 10 Dec 2021 22:12:51 GMT  
		Size: 10.9 MB (10907121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:749e3ce9b006e99a617128c15c9fcd01bf23e5eae0b3d1883f8c581047fd9797`  
		Last Modified: Fri, 10 Dec 2021 22:13:41 GMT  
		Size: 55.2 MB (55152095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e1bf0bb3aa10115e2be2311529e9c5d2a7bcd7ef41288325ff10faab16afed94
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.9 MB (137949255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f93dfdc517a48a8800f83c45292aacd0823173effab8f5a5328906da861a3b9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 02 Dec 2021 07:19:51 GMT
ADD file:b1221d684becfd74b167e24d774eb6099d264be14e0abd56599cb6a39c9eed74 in / 
# Thu, 02 Dec 2021 07:20:00 GMT
CMD ["bash"]
# Fri, 10 Dec 2021 22:17:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 10 Dec 2021 22:18:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 10 Dec 2021 22:20:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5ad94a9a32e9daafdd41e8b09d1671e7fd6b6d7cff42957db5b36cf5fe8276d1`  
		Last Modified: Thu, 02 Dec 2021 07:29:36 GMT  
		Size: 59.9 MB (59851370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190a5d1490ffcf131ea963f82913c2ec2d57ee0b6741316c88d37d687342d657`  
		Last Modified: Fri, 10 Dec 2021 22:39:49 GMT  
		Size: 5.5 MB (5543063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be29388656987e957ca7f48c588ec4c6cd00a8d2d9eee951d82efdbe540d681`  
		Last Modified: Fri, 10 Dec 2021 22:39:49 GMT  
		Size: 11.7 MB (11659256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eaac255e1eeb4950006f40a93ddcfb6c71ad56a0f1bef6ab4e9714d282401f8`  
		Last Modified: Fri, 10 Dec 2021 22:40:14 GMT  
		Size: 60.9 MB (60895566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5805da86ee2fe6eeebd93673ff1f56c488b2d26824e84c2c15221c3743031d7f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.0 MB (126043900 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44e8733ab29ecaf2699207a967ad2b82a0bccaa2c3ec6a21f1f33dc3c20535df`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 01:41:36 GMT
ADD file:c9626c75e4b53a0e71f37a2a3df45699d003ae102e7e3eedc97afe7897f82180 in / 
# Tue, 21 Dec 2021 01:41:42 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:07:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:07:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:07:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:341c5a56ba0f7b7f22f0613addb31ee3342e410686dda8753a049d0bd1f319f3`  
		Last Modified: Tue, 21 Dec 2021 01:47:23 GMT  
		Size: 53.9 MB (53888441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8be60271199953262ee02a4148a07af9a66fa017104d2d03d65d92956150fe8`  
		Last Modified: Tue, 21 Dec 2021 02:16:46 GMT  
		Size: 5.3 MB (5263047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100220edd1ab3877c378dcbe4658541db3dcee1ff143d2e1e5b5d75d67380a9b`  
		Last Modified: Tue, 21 Dec 2021 02:16:47 GMT  
		Size: 10.8 MB (10796850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68675f5371673f128e99d0c8a3b555294317faf74cbdf4da6d9b9221c2459f21`  
		Last Modified: Tue, 21 Dec 2021 02:17:01 GMT  
		Size: 56.1 MB (56095562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
