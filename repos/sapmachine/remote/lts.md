## `sapmachine:lts`

```console
$ docker pull sapmachine@sha256:77de521e810b5e718a0a4ccf38c4ac3e131149e960979d16d5b65ef3f7b7c9ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:lts` - linux; amd64

```console
$ docker pull sapmachine@sha256:ddab9afc9608acb12755de08b3b85df859878ed3bd9758af3a2f1d2b3fc83639
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.3 MB (234261919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06283a66d4d0867d3dd15507e66e3db2fd864de9bbacaa5cd4419ad2fd294ffc`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 02:30:12 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:31:17 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys CACB9FE09150307D1D22D82962754C3B3ABCFE23     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.3     && rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 02:31:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Sat, 30 Apr 2022 02:31:18 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbc4eda0a38b883dcce4c7c5d68392f244854397ca2f0cfe2a80481822fecc6`  
		Last Modified: Sat, 30 Apr 2022 02:32:08 GMT  
		Size: 7.9 MB (7925575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5535b1f22dcc4e54d805ff57601dd240bbc9f8b034a1c7dab9d54feb804895f3`  
		Last Modified: Sat, 30 Apr 2022 02:32:46 GMT  
		Size: 197.8 MB (197770114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
