## `neurodebian:non-free`

```console
$ docker pull neurodebian@sha256:485e038eac1ac7a29e7ff01c491edef99fcb2ce95d417f761b5c78e191adab6a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `neurodebian:non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:1bfc48ddb28751394a677b52f29f6053b52da3b3268334c11cf2af3c6068aed8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.6 MB (66623812 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee3f07d494cc39628a2bcf81be3c43181efc71a719b5e3fc4228602f51e46069`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Jul 2022 01:19:57 GMT
ADD file:3451708ab45bc1bcfc1ebb2075d3af16767477cbeb79334959e0d1ff02b0864b in / 
# Tue, 12 Jul 2022 01:19:58 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 04:57:31 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:57:32 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 12 Jul 2022 04:57:33 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian bullseye main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel bullseye main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 12 Jul 2022 04:57:37 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 04:57:41 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:d836772a1c1f9c4b1f280fb2a98ace30a4c4c87370f89aa092b35dfd9556278a`  
		Last Modified: Tue, 12 Jul 2022 01:24:06 GMT  
		Size: 55.0 MB (54999406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da754c27a57572208185a71b6ac71a984627b0de5c65ef03662f8dbc5272ec0e`  
		Last Modified: Tue, 12 Jul 2022 04:59:29 GMT  
		Size: 11.3 MB (11310715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9da61b5d9a6e70cf7ef7bc4d13b7baa78ca8976919df22552a39687f75732162`  
		Last Modified: Tue, 12 Jul 2022 04:59:28 GMT  
		Size: 1.8 KB (1767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8bd63f04cdfc7d5594f2e661fb39f9a0f235df8cb54f0857802e4872cf924bb`  
		Last Modified: Tue, 12 Jul 2022 04:59:28 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59532075300b5d72c0d9112603dde5e9ea7fb33b27f988295c00fa305e415f47`  
		Last Modified: Tue, 12 Jul 2022 04:59:28 GMT  
		Size: 311.3 KB (311315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd9c75058849ba530b8d8f3097aed919aa68277fce25bb396d53e0fd817bc6f`  
		Last Modified: Tue, 12 Jul 2022 04:59:40 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
