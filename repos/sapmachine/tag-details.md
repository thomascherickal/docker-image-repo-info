<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `sapmachine`

-	[`sapmachine:11`](#sapmachine11)
-	[`sapmachine:11.0.6`](#sapmachine1106)
-	[`sapmachine:13`](#sapmachine13)
-	[`sapmachine:13.0.2`](#sapmachine1302)
-	[`sapmachine:latest`](#sapmachinelatest)
-	[`sapmachine:lts`](#sapmachinelts)

## `sapmachine:11`

```console
$ docker pull sapmachine@sha256:45fae0323db5eb784072fd9f801069e9d3d53cd41545196e516d1170a87295b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sapmachine:11` - linux; amd64

```console
$ docker pull sapmachine@sha256:bdabc5d4905ba74de7d59ad326f7b159325a379c9e07213919a5791790315081
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.3 MB (231269152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b9ac2592b7f0187d50aa09e21c19fc4b0860d2cde339b0e87a7a49f8fdccc25`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:52:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:52:58 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.5     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:52:58 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Thu, 16 Jan 2020 02:52:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866b0dfbb1b590845e861921721f7536cf5350899f6c02e21e32d9c7cec9d840`  
		Last Modified: Thu, 16 Jan 2020 02:53:41 GMT  
		Size: 7.6 MB (7563739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615b703ba257ca1f088ef23cc9012722c6cc8bb575480a276cd810a7573fb6f4`  
		Last Modified: Thu, 16 Jan 2020 02:53:56 GMT  
		Size: 197.0 MB (196978845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:11.0.6`

**does not exist** (yet?)

## `sapmachine:13`

```console
$ docker pull sapmachine@sha256:bb994c14fa662cc0b08f6fcf23707b63c3ce01b343601b6a079d2ee75fe333a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sapmachine:13` - linux; amd64

```console
$ docker pull sapmachine@sha256:5dc23f22d6c0e0d3b1b72624e1b58d4949e3a65fe876e36a91291377d6a6af7e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.8 MB (241772742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65381ee32b342fa4b6bd2d1335e2c7bb146ddb46b546ebc73a6da2747ab90023`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:52:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:53:30 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-13-jdk=13.0.1     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:53:30 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-13
# Thu, 16 Jan 2020 02:53:30 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866b0dfbb1b590845e861921721f7536cf5350899f6c02e21e32d9c7cec9d840`  
		Last Modified: Thu, 16 Jan 2020 02:53:41 GMT  
		Size: 7.6 MB (7563739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652e73c8256052b1426894478c84482b8e6110cb7e9bedd9a0f0dc231e4e1100`  
		Last Modified: Thu, 16 Jan 2020 02:54:20 GMT  
		Size: 207.5 MB (207482435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:13.0.2`

**does not exist** (yet?)

## `sapmachine:latest`

```console
$ docker pull sapmachine@sha256:bb994c14fa662cc0b08f6fcf23707b63c3ce01b343601b6a079d2ee75fe333a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sapmachine:latest` - linux; amd64

```console
$ docker pull sapmachine@sha256:5dc23f22d6c0e0d3b1b72624e1b58d4949e3a65fe876e36a91291377d6a6af7e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.8 MB (241772742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65381ee32b342fa4b6bd2d1335e2c7bb146ddb46b546ebc73a6da2747ab90023`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:52:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:53:30 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-13-jdk=13.0.1     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:53:30 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-13
# Thu, 16 Jan 2020 02:53:30 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866b0dfbb1b590845e861921721f7536cf5350899f6c02e21e32d9c7cec9d840`  
		Last Modified: Thu, 16 Jan 2020 02:53:41 GMT  
		Size: 7.6 MB (7563739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652e73c8256052b1426894478c84482b8e6110cb7e9bedd9a0f0dc231e4e1100`  
		Last Modified: Thu, 16 Jan 2020 02:54:20 GMT  
		Size: 207.5 MB (207482435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `sapmachine:lts`

```console
$ docker pull sapmachine@sha256:45fae0323db5eb784072fd9f801069e9d3d53cd41545196e516d1170a87295b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sapmachine:lts` - linux; amd64

```console
$ docker pull sapmachine@sha256:bdabc5d4905ba74de7d59ad326f7b159325a379c9e07213919a5791790315081
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **231.3 MB (231269152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b9ac2592b7f0187d50aa09e21c19fc4b0860d2cde339b0e87a7a49f8fdccc25`
-	Default Command: `["jshell"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 02:52:32 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:52:58 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-11-jdk=11.0.5     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 02:52:58 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-11
# Thu, 16 Jan 2020 02:52:59 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866b0dfbb1b590845e861921721f7536cf5350899f6c02e21e32d9c7cec9d840`  
		Last Modified: Thu, 16 Jan 2020 02:53:41 GMT  
		Size: 7.6 MB (7563739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:615b703ba257ca1f088ef23cc9012722c6cc8bb575480a276cd810a7573fb6f4`  
		Last Modified: Thu, 16 Jan 2020 02:53:56 GMT  
		Size: 197.0 MB (196978845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
