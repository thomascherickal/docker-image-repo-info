## `sapmachine:latest`

```console
$ docker pull sapmachine@sha256:860eb3ea290b4eb929ad2ca34c2cc60541bd101012978dac0da4cc9edfde8994
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:latest` - linux; amd64

```console
$ docker pull sapmachine@sha256:52e6e9a0281bd2943ef06a2b547485c6aaa87118de7a74116bd16ec9cece9426
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.4 MB (248359335 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:692ef09d5ea9d008bffdb0db5b083f14a87a8c8a210658445a4c0f7ab4ad8f66`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 17 Jun 2021 23:31:29 GMT
ADD file:920cf788d1ba88f76c97e41e03e4dc2f3005b08d65b5e9da9dd1cbe20a74459b in / 
# Thu, 17 Jun 2021 23:31:29 GMT
CMD ["bash"]
# Fri, 18 Jun 2021 04:36:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:36:44 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-16-jdk=16.0.1     && rm -rf /var/lib/apt/lists/*
# Fri, 18 Jun 2021 04:36:45 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-16
# Fri, 18 Jun 2021 04:36:45 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:c549ccf8d472c3bce9ce02e49c62b8f6cbc736ea2b8ba812a1ae9390c69d0b71`  
		Last Modified: Thu, 17 Jun 2021 23:32:58 GMT  
		Size: 28.6 MB (28553692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7fe1e55c6c0fdf9092b201afb7a537d642ef9442494427e492d454dd48ae2e`  
		Last Modified: Fri, 18 Jun 2021 04:37:39 GMT  
		Size: 8.3 MB (8321832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381b68a83cc5e8d72809c48b7d08a71eba67ad98d91d427368a86e223b96b2ca`  
		Last Modified: Fri, 18 Jun 2021 04:37:54 GMT  
		Size: 211.5 MB (211483811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
