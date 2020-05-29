## `rethinkdb:2-centos`

```console
$ docker pull rethinkdb@sha256:337f58133036b1801a3a7d89bdc95e6834412fb9880ada8c0fee4c77fa715202
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `rethinkdb:2-centos` - linux; amd64

```console
$ docker pull rethinkdb@sha256:bc4ee01c40db894fa929843c6280fb3a88ef1caef3cb5065fb5170f5e2e803e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.6 MB (95607040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e91b14dfd2a34098405da55563bbe36675c5c7f603c1ad7fb5e493ddd0678ed`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 15 Jan 2020 01:19:50 GMT
ADD file:aa54047c80ba30064fe59adf4c978a929f38480be77af9ac644074bd5288ef18 in / 
# Sat, 18 Jan 2020 00:26:46 GMT
LABEL org.label-schema.schema-version=1.0 org.label-schema.name=CentOS Base Image org.label-schema.vendor=CentOS org.label-schema.license=GPLv2 org.label-schema.build-date=20200114 org.opencontainers.image.title=CentOS Base Image org.opencontainers.image.vendor=CentOS org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.created=2020-01-14 00:00:00-08:00
# Sat, 18 Jan 2020 00:26:46 GMT
CMD ["/bin/bash"]
# Fri, 29 May 2020 21:20:53 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.0
# Fri, 29 May 2020 21:20:53 GMT
RUN echo $'[rethinkdb]\nname=RethinkDB\nenabled=1\nbaseurl=https://download.rethinkdb.com/repository/centos/8/x86_64/\ngpgkey=https://download.rethinkdb.com/repository/raw/pubkey.gpg\ngpgcheck=1\n' >> /etc/yum.repos.d/rethinkdb.repo
# Fri, 29 May 2020 21:21:03 GMT
RUN yum install -y rethinkdb-$RETHINKDB_PACKAGE_VERSION 	&& yum clean all
# Fri, 29 May 2020 21:21:03 GMT
VOLUME [/data]
# Fri, 29 May 2020 21:21:03 GMT
WORKDIR /data
# Fri, 29 May 2020 21:21:03 GMT
CMD ["rethinkdb" "--bind" "all"]
# Fri, 29 May 2020 21:21:04 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:8a29a15cefaeccf6545f7ecf11298f9672d2f0cdaf9e357a95133ac3ad3e1f07`  
		Last Modified: Wed, 15 Jan 2020 01:22:13 GMT  
		Size: 73.2 MB (73228446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4ed52937dd359254212cec2ba560de303b45166cf96a4a59cf855672ffb8ae`  
		Last Modified: Fri, 29 May 2020 21:21:26 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5334e1e32012e4ef609fb934b7f8787325c38faf02a52b8dd225f98ccb3e19be`  
		Last Modified: Fri, 29 May 2020 21:21:29 GMT  
		Size: 22.4 MB (22378234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb6c71258fb5509731722064a7e271e891874f38c2f91c87e78614fb1b7e164`  
		Last Modified: Fri, 29 May 2020 21:21:26 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
