## `sapmachine:latest`

```console
$ docker pull sapmachine@sha256:7346616dfe320d37b6133864dee383aa6b87597d442b4f9c215a32f7268185a6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `sapmachine:latest` - linux; amd64

```console
$ docker pull sapmachine@sha256:f3b3fd552190fce7836cc9f77ec425379b989588bce10fbd23b925a4deb2e431
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.7 MB (246726284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56c2d9fe604e2580262b3250ee625aa3f8605667b793b999b177c356e3c23321`
-	Default Command: `["jshell"]`

```dockerfile
# Wed, 19 Aug 2020 21:14:34 GMT
ADD file:9f937f4889e7bf6467d34e7ac4f093054993a93399443dc7469d53750a62234f in / 
# Wed, 19 Aug 2020 21:14:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 19 Aug 2020 21:14:37 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 19 Aug 2020 21:14:38 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 19 Aug 2020 21:14:39 GMT
CMD ["/bin/bash"]
# Thu, 20 Aug 2020 00:51:39 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates gnupg2     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Aug 2020 00:52:05 GMT
RUN export GNUPGHOME="$(mktemp -d)"     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.old.key | gpg --batch --import     && gpg --batch --export --armor 'DA4C 00C1 BDB1 3763 8608 4E20 C7EB 4578 740A EEA2' > /etc/apt/trusted.gpg.d/sapmachine.old.gpg.asc     && wget -q -O - https://dist.sapmachine.io/debian/sapmachine.key | gpg --batch --import     && gpg --batch --export --armor 'CACB 9FE0 9150 307D 1D22 D829 6275 4C3B 3ABC FE23' > /etc/apt/trusted.gpg.d/sapmachine.gpg.asc     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb http://dist.sapmachine.io/debian/amd64/ ./" > /etc/apt/sources.list.d/sapmachine.list     && apt-get update     && apt-get -y --no-install-recommends install sapmachine-14-jdk=14.0.2     && rm -rf /var/lib/apt/lists/*
# Thu, 20 Aug 2020 00:52:05 GMT
ENV JAVA_HOME=/usr/lib/jvm/sapmachine-14
# Thu, 20 Aug 2020 00:52:05 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:54ee1f796a1e650627269605cb8e6a596b77b324e6f0a1e4443dc41def0e58a6`  
		Last Modified: Wed, 29 Jul 2020 15:19:55 GMT  
		Size: 28.6 MB (28558017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7bfea53ad120b47cea5488f0b8331e737a97b33003517b0bd05e83925b578f0`  
		Last Modified: Wed, 19 Aug 2020 21:16:56 GMT  
		Size: 32.3 KB (32336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d371e02073acecf750a166495a63358517af793de739a51b680c973fae8fb9`  
		Last Modified: Wed, 19 Aug 2020 21:16:55 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b66c17bbf772fa072c280b10fe87bc999420042b5fce5b111db38b4fe7c40b49`  
		Last Modified: Wed, 19 Aug 2020 21:16:56 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99ebeb8a0f8f5c975da8f0fa611b6b3adc22b4c86b26218d29a60b92ede1442`  
		Last Modified: Thu, 20 Aug 2020 00:52:49 GMT  
		Size: 8.3 MB (8316293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea482976c69ad797b4c04699fa1afb59c6dbac68fb30cb63d3ced06860a5c584`  
		Last Modified: Thu, 20 Aug 2020 00:53:06 GMT  
		Size: 209.8 MB (209818628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
