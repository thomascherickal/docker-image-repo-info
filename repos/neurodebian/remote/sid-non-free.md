## `neurodebian:sid-non-free`

```console
$ docker pull neurodebian@sha256:8d214312634469d3a1602f55927569503911cd14a4af62cc958ad292c173f061
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:sid-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:b7aa4b170ef3e073a51f9cd2a8d17924dd565b1c81159bc2cf96727755e89833
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64721364 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84c86ab88ea51ed31d376d90f7950a62b4c5766a025214de6988787cde4991f7`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:07:48 GMT
ADD file:51a85ad79ebd7e288cd0ea14cd2ae41990aab2d77352f801f09c3a4682cb83a9 in / 
# Fri, 11 Dec 2020 02:07:48 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 17:13:39 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 17:13:41 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Fri, 11 Dec 2020 17:13:42 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian sid main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel sid main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Fri, 11 Dec 2020 17:13:46 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 17:13:51 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:ff8cddfd21234a3c42ee0af471b251a807aa29af4ca00392976a17d3257ed269`  
		Last Modified: Fri, 11 Dec 2020 02:14:23 GMT  
		Size: 53.4 MB (53352668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2727b136c25fc091264e7b123438827cbf21b009f9c493bff195b43fe11862`  
		Last Modified: Fri, 11 Dec 2020 17:15:35 GMT  
		Size: 11.1 MB (11067345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617bbba7816c68b01e9737f10ce63810794331e00f9e16660ca78aff616e7e68`  
		Last Modified: Fri, 11 Dec 2020 17:15:34 GMT  
		Size: 1.8 KB (1760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464c117400d03f730f7dea39e3cde59a514a4eeafcc63ccb72b29be814d3a56d`  
		Last Modified: Fri, 11 Dec 2020 17:15:34 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3c7e0b6f6db759c0c88baa1dcf7186643ebb6da7f6508424e17ec4886daad3`  
		Last Modified: Fri, 11 Dec 2020 17:15:34 GMT  
		Size: 299.0 KB (299032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7cd34a181394b52b86cdf41bae92e6d92fb4ff7dae7df8f3813cad02804ad8c`  
		Last Modified: Fri, 11 Dec 2020 17:15:41 GMT  
		Size: 319.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
