## `neurodebian:focal`

```console
$ docker pull neurodebian@sha256:910dff6bf17ef9c6ecdc30982ee18bd4d09fb2c1f740e53348afde41e021eaf5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:focal` - linux; amd64

```console
$ docker pull neurodebian@sha256:39f2154d2cdb8d241fe22e1aa8d7646d29503aa842ac35aad54d97266de1598b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34302131 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db6a99a7f13a251621d206e8da7fe6bab43d65ea0af1fc7a69a8d49754a79959`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:11 GMT
ADD file:00dae10e79b05c4e1a3db053a1f85a4f38a39fe85cbbd88d74201a01a7dd59b5 in / 
# Mon, 06 Jun 2022 22:21:12 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 00:37:35 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 00:37:37 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 07 Jun 2022 00:37:37 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 07 Jun 2022 00:37:42 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7bfe07ed8476565a440c2113cc64d7c0409dba8ef761fb3ec019d7e6b5952df`  
		Last Modified: Wed, 01 Jun 2022 21:51:10 GMT  
		Size: 28.6 MB (28572632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0d85648c57095c325776ef894c7e76c557caf12f9bcb61f510da5c30f4f660`  
		Last Modified: Tue, 07 Jun 2022 00:39:47 GMT  
		Size: 5.5 MB (5489017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b42d0b055eb8b4dabb68755df18c0921420d071b554c246ac4ec6068416583`  
		Last Modified: Tue, 07 Jun 2022 00:39:46 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be77e820178f2d7d401e7cb28b70f9a90763d3bd2626132c372fec5ccbacc805`  
		Last Modified: Tue, 07 Jun 2022 00:39:46 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:885284a345938a81195044fcfc0624d73570f0df68988e21abb0a58b52e1d914`  
		Last Modified: Tue, 07 Jun 2022 00:39:46 GMT  
		Size: 238.5 KB (238469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
