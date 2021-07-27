## `sapmachine:latest`

```console
$ docker pull sapmachine@sha256:38eb44113d7d1036f44bb0d97a06b31d59c91d0bc9264effff9eb979f47727df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:latest` - linux; amd64

```console
$ docker pull sapmachine@sha256:af6aa28aedc9c07a7ae686a55abb2b3882fd49882f0481842d53eebb7934112c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.3 MB (248330928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76af2cb37fd0ebf82dc95a4fd71ca8132b1c5da106b31de5f7e02059e6c9db61`
-	Default Command: `["jshell"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:39 GMT
ADD file:524e8d93ad65f08a0cb0d144268350186e36f508006b05b8faf2e1289499b59f in / 
# Mon, 26 Jul 2021 21:21:40 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:33:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:33:33 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-16-jdk=16.0.2     && rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:33:34 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-16
# Tue, 27 Jul 2021 00:33:34 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:16ec32c2132b43494832a05f2b02f7a822479f8250c173d0ab27b3de78b2f058`  
		Last Modified: Sun, 25 Jul 2021 03:03:29 GMT  
		Size: 28.6 MB (28567944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e749eb517d141c13e9acc467b5fb1c5f84140e52ade1aca2849011c2d7a7905`  
		Last Modified: Tue, 27 Jul 2021 00:34:31 GMT  
		Size: 8.3 MB (8321704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d43919d0c53977230b7f874aa76a3c6ecf0323903cba0c99b09aa76617039df`  
		Last Modified: Tue, 27 Jul 2021 00:34:46 GMT  
		Size: 211.4 MB (211441280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
