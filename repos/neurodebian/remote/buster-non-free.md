## `neurodebian:buster-non-free`

```console
$ docker pull neurodebian@sha256:12f369eaef18b7fbb6f936ad34fd20ddf9aa361c25f5e5160074b81d6decf703
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:buster-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:3c0e2236cddaca2f0f0fae30da44146a0bafc3de4555d70dbf48bdc11ffd6263
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61259872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04d79f353601fa8661f09c7864b043a90ffe8c169b228b249899f3666aa4a9c8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 May 2023 23:47:07 GMT
ADD file:d176a72312205fc75b2950df98f4ed25abadd4b053b9d85bea67466a5b30220f in / 
# Tue, 02 May 2023 23:47:08 GMT
CMD ["bash"]
# Wed, 03 May 2023 21:25:12 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:13 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 21:25:13 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 21:25:17 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 21:25:22 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:a94073ab46f8d565f5938cc345d32f7adda10a2585e39555079da9d4ee595974`  
		Last Modified: Tue, 02 May 2023 23:50:40 GMT  
		Size: 50.4 MB (50448697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f87762e02dad34eb08994cd86e167edfd44474c49108468eb082ae17364bec7`  
		Last Modified: Wed, 03 May 2023 21:26:56 GMT  
		Size: 10.5 MB (10504492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbda83cc39ef32e5179634236082fd77e94c2021179b379bc60fc6f077b3a80`  
		Last Modified: Wed, 03 May 2023 21:26:55 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ada04c68f4b4be2aa312f558542d687e6f998884d6831a2bdee4a124b3a2cf66`  
		Last Modified: Wed, 03 May 2023 21:26:55 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd97b4a7da61a8033aa1a379b164d4f7e19016db0f734d6f6d35ed16e42cfd4`  
		Last Modified: Wed, 03 May 2023 21:26:55 GMT  
		Size: 304.3 KB (304318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b9a9a523f32160714296229f8f14f21b13da05df951a196f2f47cfa5c19b45`  
		Last Modified: Wed, 03 May 2023 21:27:04 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:12f5076aa8f8d8eccf26c7c1f5556c0d4ba106349f9f2faa6300878efd87de7a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60055702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1bebfe1e6c784ea7d1dcdd8f68728df8f8cce6fd1f2023a3bf96a1bfbc7a5c92`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 03 May 2023 00:22:56 GMT
ADD file:6042e29dcf5e22439cd69873d8960f8d3977abe915ef462aaa84368a7186a3bf in / 
# Wed, 03 May 2023 00:22:57 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:06:11 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:06:12 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 03 May 2023 19:06:12 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 03 May 2023 19:06:16 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 May 2023 19:06:19 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:b7c5fe8e0ac53c77142bf16686fc01d0d2b1fb2da7be5414cdf2f224ec485592`  
		Last Modified: Wed, 03 May 2023 00:26:10 GMT  
		Size: 49.2 MB (49238630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556cdd70aaec0c3c4f89f4a526c7171d7c63388872870c7b9df4dfcac17b8d72`  
		Last Modified: Wed, 03 May 2023 19:07:55 GMT  
		Size: 10.5 MB (10510370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fce7d4876d4114d8ba0f29c8ce008b0cd5cb525a293a4b534690f3afc1096be`  
		Last Modified: Wed, 03 May 2023 19:07:55 GMT  
		Size: 1.8 KB (1763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f9aef9aafbc896fa02484b6d34ba0e8e072897aab2e5cb1e707d34815b4958`  
		Last Modified: Wed, 03 May 2023 19:07:54 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ed33015fca163731d758e7a6bdf1201f73fe34d6a06e6f65f1707b4b3d9b72`  
		Last Modified: Wed, 03 May 2023 19:07:54 GMT  
		Size: 304.3 KB (304338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008d539b99f672e803347df1dc00483d8ae48d8d19277d32347020e11475d4ff`  
		Last Modified: Wed, 03 May 2023 19:08:03 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:9c6553053cf49f9fd5af45f0c66428de1b390291d64e9d910ee9a85358b0b403
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62380976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22b15393c4b320514bf07fcb4ceebce61357fa761cb5da1136a3b17e466dcb05`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 12 Apr 2023 00:39:11 GMT
ADD file:8299e58c7e43af1f3b9fdb9bd37e3f37cf619a97ef1b87d60ca66860d646d526 in / 
# Wed, 12 Apr 2023 00:39:11 GMT
CMD ["bash"]
# Wed, 12 Apr 2023 05:06:05 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:06:07 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 12 Apr 2023 05:06:07 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 12 Apr 2023 05:06:12 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 12 Apr 2023 05:06:14 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:2d15e1c2a3da7d675c2513d7ceab1d0f33ced9a82bed63d9a11ce71f1218d232`  
		Last Modified: Wed, 12 Apr 2023 00:43:07 GMT  
		Size: 51.2 MB (51206167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b94d9d2966b686cbabb61a0752cfddd9e119b352f4dcfc8b0705218345dcc15b`  
		Last Modified: Wed, 12 Apr 2023 05:07:29 GMT  
		Size: 10.9 MB (10868205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab36dce291d44b1a23275c0c84e5ff897b7ff86b68ee4c018b3b658a5672399`  
		Last Modified: Wed, 12 Apr 2023 05:07:27 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cfda4c6b1fab757abe0f2c8a58d6683a09f5a4d58bb3da49b51fbaaee5e3774`  
		Last Modified: Wed, 12 Apr 2023 05:07:27 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008bff0331a9b63400660f4268c8bdf6e8f5e274e5811a9173442acc3f41db05`  
		Last Modified: Wed, 12 Apr 2023 05:07:27 GMT  
		Size: 304.2 KB (304237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c48962bb79b2d164a0a95836d2525692c4f5891d64b585e7fe8ef0d358eb81f9`  
		Last Modified: Wed, 12 Apr 2023 05:07:36 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
