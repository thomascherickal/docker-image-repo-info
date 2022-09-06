## `couchbase:community-6.6.0`

```console
$ docker pull couchbase@sha256:4a6e08017eee1cdb4718699906af761265ece7d36d1bd92ff448af26899e02d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-6.6.0` - linux; amd64

```console
$ docker pull couchbase@sha256:1245176b91d008575575cd3fd38cc48554a65769e67f0a910f1e3ee4003f815b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.5 MB (352537747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7efb0684b1c8436e4552c90ce9f93975c1b10e42fa8e9f0780a2fa45bed5662`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 06 Sep 2022 19:38:36 GMT
ADD file:8733c7e8faf03d53cb2143ff6ac405362944cfa07422fccd21a3066cc2f42c83 in / 
# Tue, 06 Sep 2022 19:38:37 GMT
CMD ["bash"]
# Tue, 06 Sep 2022 20:05:12 GMT
LABEL maintainer=docker@couchbase.com
# Tue, 06 Sep 2022 20:05:12 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Tue, 06 Sep 2022 20:05:12 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Tue, 06 Sep 2022 20:05:29 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Tue, 06 Sep 2022 20:05:29 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Tue, 06 Sep 2022 20:05:29 GMT
ARG CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb
# Tue, 06 Sep 2022 20:05:29 GMT
ARG CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559
# Tue, 06 Sep 2022 20:05:29 GMT
ARG CB_SKIP_CHECKSUM=false
# Tue, 06 Sep 2022 20:05:29 GMT
ARG CB_PACKAGE_NAME=couchbase-server-community
# Tue, 06 Sep 2022 20:05:30 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Tue, 06 Sep 2022 20:05:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Tue, 06 Sep 2022 20:06:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && dpkg --unpack ./$CB_PACKAGE     && sed -i -e '/Best heuristic/ a \ \ \ \ [ -d /run/systemd/system ] && return 1; return 0' /opt/couchbase/bin/install/systemd-ctl     && dpkg --configure couchbase-server-community     && apt-get install -yf     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Tue, 06 Sep 2022 20:06:11 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Tue, 06 Sep 2022 20:06:11 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Tue, 06 Sep 2022 20:06:11 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Tue, 06 Sep 2022 20:06:11 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Tue, 06 Sep 2022 20:06:12 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Tue, 06 Sep 2022 20:06:20 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Tue, 06 Sep 2022 20:06:20 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Tue, 06 Sep 2022 20:06:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 06 Sep 2022 20:06:21 GMT
CMD ["couchbase-server"]
# Tue, 06 Sep 2022 20:06:21 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Tue, 06 Sep 2022 20:06:21 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:726b8a513d66e3585eb57389171d97fcd348e4914a415891e1da135b85ffa6c3`  
		Last Modified: Fri, 02 Sep 2022 15:41:13 GMT  
		Size: 26.7 MB (26710833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6ea2f5eb60935a281e599e8a48eda7001b9cadc55c86ad643aa3840659944a`  
		Last Modified: Tue, 06 Sep 2022 20:07:02 GMT  
		Size: 5.6 MB (5625899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2011525723328cc2a0aead0a47cafbcf30e27b8878618e975d127ff68f5e479`  
		Last Modified: Tue, 06 Sep 2022 20:07:00 GMT  
		Size: 2.0 KB (1968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0308e4d0a928ca2953ea88f26f4743e86a1c9290148c1881527ce9d15193e4`  
		Last Modified: Tue, 06 Sep 2022 20:07:36 GMT  
		Size: 319.8 MB (319763162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3dedc57c499e50368dee35afde3e0a508ee496f4a444cbc848eb486488ca51`  
		Last Modified: Tue, 06 Sep 2022 20:07:00 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bdb98ab4ae420b6a09020a9b7b9b813cb83395f8470e2e069fa93b808dd330c`  
		Last Modified: Tue, 06 Sep 2022 20:07:00 GMT  
		Size: 742.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60204c1bbf678ee089fbac09a46466be01fec0ea7fbfab51b37e1c0a2f81b634`  
		Last Modified: Tue, 06 Sep 2022 20:06:58 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06bc3fc4be8bb43fcfa7609227c1abd783a7c9a0c82ff4920168d7dd80a44fd`  
		Last Modified: Tue, 06 Sep 2022 20:06:58 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa60c950d227e28972a9217f8f213190fc95f85fa50f4b6ba7de921a9ade0bd4`  
		Last Modified: Tue, 06 Sep 2022 20:06:58 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9874cfb6e26e5e3c4d06166d8acb8f53b228fd2f4e222c4e9d0a2990e8d1bb94`  
		Last Modified: Tue, 06 Sep 2022 20:06:58 GMT  
		Size: 433.4 KB (433352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df825d9d16f6f599a3316de0ee6f7f7bd831d0b025fb3155faf02ceb23095f`  
		Last Modified: Tue, 06 Sep 2022 20:06:58 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
