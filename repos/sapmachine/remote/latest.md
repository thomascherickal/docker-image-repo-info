## `sapmachine:latest`

```console
$ docker pull sapmachine@sha256:c45e13060f0d983af01990843eb7afcc7759dc078a4274d89a33ae216a6db69a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:latest` - linux; amd64

```console
$ docker pull sapmachine@sha256:53a036f4d787126777c010437ee4802de11b193e8aca556170301ab2c2359bc6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **235.2 MB (235238782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c41946584fd5f135ac2d29893bf5075e90fa394324df6f6638cf806a8bfdb4d6`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 21 Apr 2022 23:00:07 GMT
ADD file:064c61cc9ceed678689d2eaf3b3e61ec3bf5baf9288e5a7febcbab28c6adbfb6 in / 
# Thu, 21 Apr 2022 23:00:07 GMT
CMD ["bash"]
# Fri, 22 Apr 2022 03:56:59 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Apr 2022 18:45:26 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-18-jdk=18.0.1     && rm -rf /var/lib/apt/lists/*
# Mon, 25 Apr 2022 18:45:26 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-18
# Mon, 25 Apr 2022 18:45:26 GMT
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
	-	`sha256:e51f54a7768db62b805938bea93643015d7116f6c6058cadc538d19265b256da`  
		Last Modified: Mon, 25 Apr 2022 18:46:53 GMT  
		Size: 198.7 MB (198747263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
