## `sapmachine:lts`

```console
$ docker pull sapmachine@sha256:39c50779b7b8eb1e6482fcf9eb395891c430d3bd145883e8ca156ea3a9d9a8c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:lts` - linux; amd64

```console
$ docker pull sapmachine@sha256:bc044fc214cc5c429e3593786560078654e9481d91e29fcf3cfef03c865f9de2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.5 MB (234531275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:904eeec7bd063c5bc435c15c588e3f4e50c40a7834cc9c8fb802d3de6c944122`
-	Default Command: `["jshell"]`

```dockerfile
# Fri, 07 Jan 2022 02:25:29 GMT
ADD file:122ad323412c2e70b3138d8eb62648c4692989de91be1ffb6b4bf086c8311b62 in / 
# Fri, 07 Jan 2022 02:25:30 GMT
CMD ["bash"]
# Fri, 07 Jan 2022 03:52:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 04:21:19 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17.0.2     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Jan 2022 04:21:20 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Thu, 20 Jan 2022 04:21:20 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:ea362f368469f909a95f9a6e54ebe0121ce0a8e3c30583dd9c5fb35b14544dec`  
		Last Modified: Thu, 06 Jan 2022 15:07:12 GMT  
		Size: 28.6 MB (28566425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36523c5bf0a6824c09aef7ff4add53bfee4d51934121d0c840861937bec44467`  
		Last Modified: Fri, 07 Jan 2022 03:54:03 GMT  
		Size: 8.3 MB (8318485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdfb3c81b002e170798b95135bec75f773114b28621fce6cea84aec57cd3eb30`  
		Last Modified: Thu, 20 Jan 2022 04:22:19 GMT  
		Size: 197.6 MB (197646365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
