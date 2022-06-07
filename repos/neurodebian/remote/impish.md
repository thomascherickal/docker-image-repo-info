## `neurodebian:impish`

```console
$ docker pull neurodebian@sha256:7aaf8441df1e42705456bbd66f50bacdc3dbebdacc47c7bd4683c5666e25a836
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:impish` - linux; amd64

```console
$ docker pull neurodebian@sha256:db1963ee159e0dca0159562742ad532d2a086a988b9354057ed8d77647b5e0f8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34384580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57e017fc712553f899766998fdb9db30eee355df9033c23dd72ba12b43aa47eb`
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
