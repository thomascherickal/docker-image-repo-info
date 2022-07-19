## `neurodebian:impish-non-free`

```console
$ docker pull neurodebian@sha256:d8dd2cc8165345590b62af26fc7a2e0df2f5060d4450b4610e7b6b23517f1535
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `neurodebian:impish-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:fa54f734923cf3bc814f9ca42375869480681699d414e88acb6e22b84dc40570
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34384840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a47ecb4e0e0a6f4fa722091c451eb400637d32dcf1bb57d808dcb0e1b55c994`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:18 GMT
ADD file:d6b83520d39d5b64128115fc97a16a462c38d8e06ef69baad724eda9da91f934 in / 
# Mon, 06 Jun 2022 22:21:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:38:13 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:38:14 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 07 Jun 2022 00:38:15 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian impish main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel impish main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 07 Jun 2022 00:38:19 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 19:53:52 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:54b8fda3c9de3a40f0891ce200de55fc92e825315021192957f1bfe3fc807d7d`  
		Last Modified: Mon, 06 Jun 2022 22:22:48 GMT  
		Size: 30.4 MB (30380290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4222215fe5bb0924cc9cbcbbb6d524fc181c91b66bd31430a258a78ebce2c519`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 3.8 MB (3752244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983039d4e1a2415f0f809ddd83bcc60a90fe40cf2e2c3a4f93ded36ac4cab37a`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 1.8 KB (1765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d378c9cd6485d098e5bcf609a3e34edc5c31a424035a4bd61de01eadbab71c6`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e2ecd075adf7f432e69fbe49ea1b42a7c15c0cf6114789b57ffa534f851834`  
		Last Modified: Tue, 07 Jun 2022 00:40:06 GMT  
		Size: 250.0 KB (250036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89cf61727686c8d90437ef15476fa41e9fb4a62ac20103873c80d2c3a11c3f3b`  
		Last Modified: Tue, 19 Jul 2022 19:57:02 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:impish-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:d4317d75f7993f1c0989813fb01ddb8c37b2c45f469d348b3f06cf10fb4fc29e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32856749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2014687e1f50bb858f914f8177891ca3949ae87fc8fbbd65b7b1a140b43d7e70`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:24 GMT
ADD file:d1932d13ea73e26ad39647db09c23895cf0644ba34851cb87e777778d59b6730 in / 
# Tue, 07 Jun 2022 01:25:24 GMT
CMD ["bash"]
# Tue, 19 Jul 2022 20:09:24 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 20:09:26 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Jul 2022 20:09:27 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian impish main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel impish main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Jul 2022 20:10:09 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Jul 2022 20:10:16 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list; grep -q 'deb .* multiverse$' $srcs || sed -i -e 's,universe *$,universe multiverse,g' $srcs
```

-	Layers:
	-	`sha256:166e0294b8df947d819744f38e21281ed5f29a2a3b19d191deee511cbfb0e473`  
		Last Modified: Tue, 07 Jun 2022 01:27:26 GMT  
		Size: 29.0 MB (29018061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fd390207922789eacc8378770b82705bf3ef6a8ee15ff29c896c4c7b3a8737`  
		Last Modified: Tue, 19 Jul 2022 20:15:09 GMT  
		Size: 3.7 MB (3726896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41123559e445d7fd43518edd8d4445a77c75c6fed0745b660394be39800e2e06`  
		Last Modified: Tue, 19 Jul 2022 20:15:07 GMT  
		Size: 1.7 KB (1743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3949fbe2cfc1efed7983069b8e05e484d5bbe3334f54d1142a5bbb1dff8d3f`  
		Last Modified: Tue, 19 Jul 2022 20:15:07 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7168a0a709927f8d07cdd160accd5040d26e868fb92cc598d965c3654d28c3f`  
		Last Modified: Tue, 19 Jul 2022 20:15:08 GMT  
		Size: 109.5 KB (109547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e2bd7e7df381379f1dde19c12b40e93e765871170afe519be5f19b996972af`  
		Last Modified: Tue, 19 Jul 2022 20:15:19 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
