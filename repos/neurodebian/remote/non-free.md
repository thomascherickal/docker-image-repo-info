## `neurodebian:non-free`

```console
$ docker pull neurodebian@sha256:13a3ae717588d73d1d91a3f997209fc927701801068aa69c46d26eef457f3939
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `neurodebian:non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:917edfa4143b97d15a361baca32e01405cf22c3c2e1e6b2dc8d0c196fa9b775b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61200549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4005d67eed11091e26c769248175261693ae56fd9d3d6bbeb40ba2965eafb7c3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:05:52 GMT
ADD file:6014cd9d7466825f80d4a3345847efd6fd7ef600b8135811cab4f0e304f66cd7 in / 
# Fri, 11 Dec 2020 02:05:52 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 17:12:52 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 17:12:53 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Fri, 11 Dec 2020 17:12:54 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Fri, 11 Dec 2020 17:12:58 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 17:13:04 GMT
RUN sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list /etc/apt/sources.list
```

-	Layers:
	-	`sha256:6c33745f49b41daad28b7b192c447938452ea4de9fe8c7cc3edf1433b1366946`  
		Last Modified: Fri, 11 Dec 2020 02:12:07 GMT  
		Size: 50.4 MB (50397728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6c66699048e52432819f9112d0e4b7f96214e221978455d6b0b03b0da33342e`  
		Last Modified: Fri, 11 Dec 2020 17:15:11 GMT  
		Size: 10.5 MB (10497948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0303af6cf2347aeb70ef9a23a7c4be666d35d14fddf1c2d81790bb35f8ac4a25`  
		Last Modified: Fri, 11 Dec 2020 17:15:10 GMT  
		Size: 1.8 KB (1757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726d52d9a1e530d78590b2b3bfe3bf0b22d178caa9a5b2618823d4840fbebe41`  
		Last Modified: Fri, 11 Dec 2020 17:15:10 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6b82482aaca0612234b7f4945ef4c4804eadc900afcbd5b30589006f175de3e`  
		Last Modified: Fri, 11 Dec 2020 17:15:10 GMT  
		Size: 302.5 KB (302504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00739c9533012cde6c9d655074328bc2cc018efbc85e2a3bc98cda4048d7fe8a`  
		Last Modified: Fri, 11 Dec 2020 17:15:17 GMT  
		Size: 369.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
