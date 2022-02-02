## `sapmachine:latest`

```console
$ docker pull sapmachine@sha256:0b6cc527565863e89be806c1ea9170ff5a40166bacc545202cab39c371d676d8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:latest` - linux; amd64

```console
$ docker pull sapmachine@sha256:8ec0fb4bd7c43b5cd0e7f37e3c5657d217dd17e39863c5e936fd5d7e32a4141d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.5 MB (234528762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61a8d0d46286e3ce9dd024a48d09794eb0e30dc21d184310c7716cbb0f17691c`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 02 Feb 2022 02:14:45 GMT
ADD file:3ccf747d646089ed7fbb43c40c45dd43e86f0674115f856efada93c7e4a63624 in / 
# Wed, 02 Feb 2022 02:14:46 GMT
CMD ["bash"]
# Wed, 02 Feb 2022 07:04:35 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 07:05:40 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.2     && rm -rf /var/lib/apt/lists/*
# Wed, 02 Feb 2022 07:05:41 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Wed, 02 Feb 2022 07:05:41 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:08c01a0ec47e82ebe2bec112f373d160983a6d1e9e66627f66a3322bc403221b`  
		Last Modified: Wed, 02 Feb 2022 02:16:20 GMT  
		Size: 28.6 MB (28564099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62164c5b3eea6ba9e40ab7adbcb5b8d492e8c8c0c763bd36f36cf58c59f3ee7b`  
		Last Modified: Wed, 02 Feb 2022 07:05:57 GMT  
		Size: 8.3 MB (8318363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a697cbcafa0887e827a76bd669fb29aa4669f08023ea93d5575254618edc84a`  
		Last Modified: Wed, 02 Feb 2022 07:06:34 GMT  
		Size: 197.6 MB (197646300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
