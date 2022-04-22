## `neurodebian:focal`

```console
$ docker pull neurodebian@sha256:2e986f332c0a5fd4bb3e469f8802b4097f4967aac5559d8dd5dde160a077904c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:focal` - linux; amd64

```console
$ docker pull neurodebian@sha256:eef6fada6a01fd01b68dfe4301b1d1c7d71a7e1002c0a23adfb4197675a7e00d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34294628 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdf11550e4931d6195fce35fde7000ff93ca5e4823eb94111d35c5e5bb8e202f`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 02:59:32 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 02:59:33 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Fri, 22 Apr 2022 02:59:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian focal main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel focal main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Fri, 22 Apr 2022 02:59:38 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea1a7fa2a5ae0557cb0a65c8beb62c914826380d29676bf6f7319a31a9b9280`  
		Last Modified: Fri, 22 Apr 2022 03:01:43 GMT  
		Size: 5.5 MB (5488521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c959804ab2aaec4aa1e6d1fedfe83beee2950f1e67133be10eff98d547bc00ad`  
		Last Modified: Fri, 22 Apr 2022 03:01:43 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0addefcc93ea0efefa4b94cb383e92c0ab2c3ef0e9f4323e89ddb3e66bdba41a`  
		Last Modified: Fri, 22 Apr 2022 03:01:42 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c30a144e057992438aea7802ec2b9ece08b19ff6a73c237ec30f9db1f3e0a2a`  
		Last Modified: Fri, 22 Apr 2022 03:01:42 GMT  
		Size: 238.1 KB (238096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
