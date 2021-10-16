## `sapmachine:lts`

```console
$ docker pull sapmachine@sha256:b2d20a973f5709fdc20f8a80254350a88e2f179b2af0606a971f1bd5e47c3e99
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `sapmachine:lts` - linux; amd64

```console
$ docker pull sapmachine@sha256:dffcc4440ea537dbd347c6e21113618772480fb479f1dae7e8dee56e233af3b5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.5 MB (234474179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90902f79da9973a2558566e38ad2411a21c69ca3a1e99a5780ebc7d196215f44`
-	Default Command: `["jshell"]`

```dockerfile
# Sat, 16 Oct 2021 00:37:47 GMT
ADD file:5d68d27cc15a80653c93d3a0b262a28112d47a46326ff5fc2dfbf7fa3b9a0ce8 in / 
# Sat, 16 Oct 2021 00:37:47 GMT
CMD ["bash"]
# Sat, 16 Oct 2021 02:09:19 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:10:27 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-17-jdk=17     && rm -rf /var/lib/apt/lists/*
# Sat, 16 Oct 2021 02:10:28 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-17
# Sat, 16 Oct 2021 02:10:28 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:7b1a6ab2e44dbac178598dabe7cff59bd67233dba0b27e4fbd1f9d4b3c877a54`  
		Last Modified: Thu, 07 Oct 2021 23:44:23 GMT  
		Size: 28.6 MB (28567101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25367b1bc88dc85c34043fc951848985a61bfa2247f9e88d7cf4b4ce551f4d8`  
		Last Modified: Sat, 16 Oct 2021 02:10:41 GMT  
		Size: 8.3 MB (8319595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7617e847a51233fe2fce520997755abc64b58c359c956427d600a395705d1c5`  
		Last Modified: Sat, 16 Oct 2021 02:11:18 GMT  
		Size: 197.6 MB (197587483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
