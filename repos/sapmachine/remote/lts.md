## `sapmachine:lts`

```console
$ docker pull sapmachine@sha256:88c3de8563dc272094dc80ae598018e104ee75ecb0314ab4d6c3cd39110a8f37
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:lts` - linux; amd64

```console
$ docker pull sapmachine@sha256:5598734eee25203dd624c283f41e4850ce5bab95dda33d5434037f96c4d6bbae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234261660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:167950fcad87f9159b1ad1d6c930ae8072a460efb74027fd6957b798f4648dd2`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:56:59 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Apr 2022 18:44:46 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.3     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Apr 2022 18:44:47 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Mon, 25 Apr 2022 18:44:47 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:8e5c1b329fe39c318c0d49821b339fb94a215c5dc0a2898c8030b5a4d091bcba`  
		Last Modified: Sun, 17 Apr 2022 03:03:46 GMT  
		Size: 28.6 MB (28565998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb3497eded1e3eecf8f2698c510b36e1d91b42337d37bd2dc6e64189ae252b6`  
		Last Modified: Fri, 22 Apr 2022 03:58:43 GMT  
		Size: 7.9 MB (7925521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce79242b5f06b6b44eeb2ba776c7ed660af8069d9625639391cd948169df38c4`  
		Last Modified: Mon, 25 Apr 2022 18:46:25 GMT  
		Size: 197.8 MB (197770141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
