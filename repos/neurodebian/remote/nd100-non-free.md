## `neurodebian:nd100-non-free`

```console
$ docker pull neurodebian@sha256:9aa278543265ea7036c3b624ad84467bc50c6e373a0595adda8adec37b74cb1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:nd100-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:36baea0d92be742ffacd3e287f3aff751161983cafac9656a231765c900b5b34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61258767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c289b0f5dc037a7f60cd95e66a73e31a506be771f2aaf96d656292db28d88c5f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 01:44:02 GMT
ADD file:259be79d94a2549a667ad08a093fe18f15a6c93d66a0723292f49294e31fc7a1 in / 
# Tue, 25 Oct 2022 01:44:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 04:13:07 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:13:09 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 25 Oct 2022 04:13:09 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 25 Oct 2022 04:13:14 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 04:13:18 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:fd31ec14dccdcda8f2472547f1a94ef0a23b8dabb764cd7b1d48aeee0afea7c8`  
		Last Modified: Tue, 25 Oct 2022 01:48:15 GMT  
		Size: 50.4 MB (50447742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9122ec6aa2a6194ca00862c6d9350bc5b3a8b530dfdf48dd3973cac441ddb49f`  
		Last Modified: Tue, 25 Oct 2022 04:15:59 GMT  
		Size: 10.5 MB (10504344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c4c20cf0b981052b23457bc1f8457f68bd7515cad276917ba46fb57144c755d`  
		Last Modified: Tue, 25 Oct 2022 04:15:58 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb9a440939dfe96a44b07dfa89426581578c53b5e5d02c8b8b02b74d3fc9305`  
		Last Modified: Tue, 25 Oct 2022 04:15:58 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879b3b855360c632fcecd2c95dd76c57425ff8bb0dc3e9d94794896068a07ebf`  
		Last Modified: Tue, 25 Oct 2022 04:15:59 GMT  
		Size: 304.3 KB (304315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ae27cf1fad4a72965222c9604eb452c169583c3844584aafc24d68824bf812`  
		Last Modified: Tue, 25 Oct 2022 04:16:08 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:ae50d50c11c32068f7b0f868f8975041e8cc6381108233aa6926e8f2b4dbb863
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.6 MB (59637153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e1ca9d0cf271394b943e6c4dbc574cc3b61dbe9eed4fa82dbd4e4feaf92085c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:54 GMT
ADD file:ef2ee78fb3eda698ebec33ff4b6dea672e03908b0f8630a28acb33ec9a7c3e13 in / 
# Tue, 04 Oct 2022 23:44:55 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:58:26 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:28 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Wed, 05 Oct 2022 03:58:29 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Wed, 05 Oct 2022 03:58:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:58:40 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:504dcdd9b4a0035dba7a55a5312cf594c3d22fb99b7bf676d397c464db919009`  
		Last Modified: Tue, 04 Oct 2022 23:50:47 GMT  
		Size: 49.2 MB (49228885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d154496b8ab72771340bbbfcb90129abefba06a0df134e694e436c32723ecf`  
		Last Modified: Wed, 05 Oct 2022 04:02:31 GMT  
		Size: 10.3 MB (10297436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef89a9a6d8113e10f9e579ee92783e306a5fa8bfe2acfa01e2d78d7fd818107f`  
		Last Modified: Wed, 05 Oct 2022 04:02:29 GMT  
		Size: 1.7 KB (1741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23704a18d02fdbc4131c6f7adfaaec3730093c5504d02a143c4a78f637028721`  
		Last Modified: Wed, 05 Oct 2022 04:02:29 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d322400769bb470d58b21b11c9f6e84fb73d5e8603c40127b4804943ec7f7ec2`  
		Last Modified: Wed, 05 Oct 2022 04:02:30 GMT  
		Size: 108.5 KB (108492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ebd81db9bac845b1da95a5029d74042c0045701de4248a1c4a035311b28efe`  
		Last Modified: Wed, 05 Oct 2022 04:02:41 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:nd100-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:c81c4b4acdd2b5d5a0dd45be0cc006bd9e2831ea34682274356bbe5e5385a50a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.0 MB (61991387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b22776d8442dbe8efdfe950fbf3a05109418803993a8cb77bd37c5ecffe50e9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 25 Oct 2022 02:22:47 GMT
ADD file:7e14d4afa5499129c959c5ae5dc270e2fa04659c2c9b0527094cda3494c02d0f in / 
# Tue, 25 Oct 2022 02:22:47 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 11:42:09 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 11:42:11 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 25 Oct 2022 11:42:12 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 25 Oct 2022 11:42:17 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 11:42:23 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:76a731c42f665e7334a622f65117ef9389e97a878b7c74bb4a10dfe9cdb296c6`  
		Last Modified: Tue, 25 Oct 2022 02:28:50 GMT  
		Size: 51.2 MB (51207943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abadbaf3845d089c8fd53b5ffd40578cd54908ba95316e30fdf09a54cf6869a`  
		Last Modified: Tue, 25 Oct 2022 11:44:30 GMT  
		Size: 10.7 MB (10672420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0a3a5da4addd1e47a5b69c36f6012ef4f287a67d886bc5c6f9130b3b7f777a`  
		Last Modified: Tue, 25 Oct 2022 11:44:29 GMT  
		Size: 1.7 KB (1739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d780340726e09c5c713d4b88312efd8981d14499e5157a5b17998311301a19`  
		Last Modified: Tue, 25 Oct 2022 11:44:29 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb95c64d458e9fa11783ca64bd98411613979fe50034c8d54c829b602b69d541`  
		Last Modified: Tue, 25 Oct 2022 11:44:29 GMT  
		Size: 108.7 KB (108686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:835bc82fa14cf3103b870462edebd97cbfcb7f89016fd96f134fa3efb804ec5f`  
		Last Modified: Tue, 25 Oct 2022 11:44:40 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
