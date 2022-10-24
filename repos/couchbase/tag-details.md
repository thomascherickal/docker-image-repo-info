<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchbase`

-	[`couchbase:6.6.5`](#couchbase665)
-	[`couchbase:7.0.4`](#couchbase704)
-	[`couchbase:7.1.2`](#couchbase712)
-	[`couchbase:community`](#couchbasecommunity)
-	[`couchbase:community-6.6.0`](#couchbasecommunity-660)
-	[`couchbase:community-7.0.2`](#couchbasecommunity-702)
-	[`couchbase:community-7.1.1`](#couchbasecommunity-711)
-	[`couchbase:enterprise`](#couchbaseenterprise)
-	[`couchbase:enterprise-6.6.5`](#couchbaseenterprise-665)
-	[`couchbase:enterprise-7.0.4`](#couchbaseenterprise-704)
-	[`couchbase:enterprise-7.1.2`](#couchbaseenterprise-712)
-	[`couchbase:latest`](#couchbaselatest)

## `couchbase:6.6.5`

```console
$ docker pull couchbase@sha256:f1ed8218ba5b59fb643e32966f9e834cd8cf969c571e16a64e3bf397a3ae4394
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:6.6.5` - linux; amd64

```console
$ docker pull couchbase@sha256:e5cc2084694132e099f7640c314f52e8733bcad173b2553ebb5342123053305d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **540.9 MB (540902425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b16ba5ebc72018eb36e6dd59cd9d20f78d7686b96869002e952c0026308f74`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:43:58 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 05 Oct 2022 16:43:58 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 05 Oct 2022 16:43:58 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 05 Oct 2022 16:44:32 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 05 Oct 2022 16:49:27 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5
# Wed, 05 Oct 2022 16:49:27 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb
# Wed, 05 Oct 2022 16:49:27 GMT
ARG CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6
# Wed, 05 Oct 2022 16:49:27 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 05 Oct 2022 16:49:27 GMT
ARG CB_PACKAGE_NAME=couchbase-server
# Wed, 05 Oct 2022 16:49:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 05 Oct 2022 16:49:28 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 05 Oct 2022 16:50:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && dpkg --unpack ./$CB_PACKAGE     && sed -i -e '/Best heuristic/ a \ \ \ \ [ -d /run/systemd/system ] && return 1; return 0' /opt/couchbase/bin/install/systemd-ctl     && dpkg --configure couchbase-server     && apt-get install -yf     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 05 Oct 2022 16:50:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 05 Oct 2022 16:50:23 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 05 Oct 2022 16:50:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 05 Oct 2022 16:50:24 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 05 Oct 2022 16:50:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 05 Oct 2022 16:50:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 05 Oct 2022 16:50:31 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 05 Oct 2022 16:50:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 16:50:31 GMT
CMD ["couchbase-server"]
# Wed, 05 Oct 2022 16:50:31 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 05 Oct 2022 16:50:32 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f6521e7788616a3d54de1df237a477200baa4fcdcbc80f1ca20102c8dac9a2`  
		Last Modified: Wed, 05 Oct 2022 16:52:36 GMT  
		Size: 6.2 MB (6232202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18dd9c54682a90764bcd4ab2ea200d80fccb8d87501195e6611a9b6b410f6505`  
		Last Modified: Wed, 05 Oct 2022 16:56:56 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5affd3fa6a36992a447da553db74ba262aea2c14198d0c1d470b8b6eab16d888`  
		Last Modified: Wed, 05 Oct 2022 16:57:49 GMT  
		Size: 505.7 MB (505651775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10c297192bd86a2c0f056b6ac8204ef405238d034f694279475f66e53967be9`  
		Last Modified: Wed, 05 Oct 2022 16:56:56 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8f4ec6103f66664911ae3c569a7c49c826f0563488b7b6c35d36a7a5609deb`  
		Last Modified: Wed, 05 Oct 2022 16:56:56 GMT  
		Size: 738.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e3bce98c83822f6ee9604fc88a7b4bfe84d64c7cf771396f8b9d6bed7cf413`  
		Last Modified: Wed, 05 Oct 2022 16:56:54 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8788b0f02f82a694f4d429b38c3823e038f77b4ffd60aa97bcdc94a89cd9b372`  
		Last Modified: Wed, 05 Oct 2022 16:56:54 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6def2a48c9d2562a5bf5b839a8f640634a75413dd351ae7323d0c7c9a94a093`  
		Last Modified: Wed, 05 Oct 2022 16:56:54 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4323301d29d5923422b1f072ff6a1338ba9f893c9226a19e0a1b03d2c13ea540`  
		Last Modified: Wed, 05 Oct 2022 16:56:55 GMT  
		Size: 439.6 KB (439628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262160f2dba6a58a826580627d7887a70a0ad12d71b1b05842f0f5747231035d`  
		Last Modified: Wed, 05 Oct 2022 16:56:54 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:7.0.4`

```console
$ docker pull couchbase@sha256:6fb17f745b5d12f7986b1f71092210e186b836ac6d1f29158288d681d2473154
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:7.0.4` - linux; amd64

```console
$ docker pull couchbase@sha256:bb6b822e4a36e770aedf2c084e3872fd3088591e51891fdf33c79dca344e2f1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **641.1 MB (641145367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61698097571dc39f0348f6088aad6ff50d956002bd50643ec71d558e422189a6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:43:58 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 05 Oct 2022 16:43:58 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 05 Oct 2022 16:43:58 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 05 Oct 2022 16:44:32 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Mon, 24 Oct 2022 21:27:39 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4
# Mon, 24 Oct 2022 21:27:39 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb
# Mon, 24 Oct 2022 21:27:39 GMT
ARG CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2
# Mon, 24 Oct 2022 21:27:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 24 Oct 2022 21:27:40 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4 CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 24 Oct 2022 21:28:50 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4 CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c -     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:28:55 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4 CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 24 Oct 2022 21:28:55 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Mon, 24 Oct 2022 21:28:56 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4 CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 24 Oct 2022 21:28:56 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 24 Oct 2022 21:28:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4 CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 24 Oct 2022 21:29:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4 CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Mon, 24 Oct 2022 21:29:05 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Mon, 24 Oct 2022 21:29:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Oct 2022 21:29:05 GMT
CMD ["couchbase-server"]
# Mon, 24 Oct 2022 21:29:05 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 24 Oct 2022 21:29:05 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f6521e7788616a3d54de1df237a477200baa4fcdcbc80f1ca20102c8dac9a2`  
		Last Modified: Wed, 05 Oct 2022 16:52:36 GMT  
		Size: 6.2 MB (6232202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecab90dac59c107f5dd70235be20f72b55b47b158f63b47125d6c0fd191ca930`  
		Last Modified: Mon, 24 Oct 2022 21:30:57 GMT  
		Size: 1.8 KB (1845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd53ad08efa52facea1982c7bdc350701fbf18f07001d6473ff093e2964d3be`  
		Last Modified: Mon, 24 Oct 2022 21:32:30 GMT  
		Size: 605.9 MB (605890340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df565d7527eb8d41cd1662a1635d93b007ec3384e31eaa21b8cf26304206a5d`  
		Last Modified: Mon, 24 Oct 2022 21:30:57 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b846649aa7e9275d1385f3ac587ced227eb211415c82da98d27118a8f46b29`  
		Last Modified: Mon, 24 Oct 2022 21:30:57 GMT  
		Size: 744.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d227861109fc824e1e97687726cdf9ef1d92b5a0d6c27e8e0c61be9fce5261`  
		Last Modified: Mon, 24 Oct 2022 21:30:55 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bc438f6eaf8ccd9d706a6400206b43a40ffe96eefb61dd25f74183d435a8f2`  
		Last Modified: Mon, 24 Oct 2022 21:30:55 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646ea57d4f974ef19e4e88ae9745b730a3c3cb2cc75a304474c66d0ad871022e`  
		Last Modified: Mon, 24 Oct 2022 21:30:55 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a8989065f3279985c667aaa8eb0ec3420dc0db82c225e04dade8238dd9459d`  
		Last Modified: Mon, 24 Oct 2022 21:30:55 GMT  
		Size: 444.0 KB (443988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59389ff2f8c5cfc0bf8b97dce5b001f6f2bb88230bfb119146071c5144bba1c9`  
		Last Modified: Mon, 24 Oct 2022 21:30:55 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:7.1.2`

```console
$ docker pull couchbase@sha256:fb14ff77878dcc2f53b40764d8b7413268026a3a52d04ed3a06fede454e64d8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:7.1.2` - linux; amd64

```console
$ docker pull couchbase@sha256:43db9f11908feafb47719a0e926bfb3875efa4eb34bf233856b7e3a75778c2e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **600.1 MB (600052223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a4e33350b160e36ed40a8ffe8424cfb308dad94279fa3e50445693d7666352`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:43:58 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 05 Oct 2022 16:43:58 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 05 Oct 2022 16:43:58 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 05 Oct 2022 16:44:32 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Mon, 24 Oct 2022 21:25:59 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2
# Mon, 24 Oct 2022 21:25:59 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb
# Mon, 24 Oct 2022 21:25:59 GMT
ARG CB_SKIP_CHECKSUM=false
# Mon, 24 Oct 2022 21:25:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 24 Oct 2022 21:26:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 24 Oct 2022 21:27:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=1c7c757cf8aee87b98c96ffea1c26f4c98b6e0c053d966c8e760224030d98477            ;;          'amd64')            CB_SHA256=26fd9ae8585e0ea6637d4f1b492ed637dcf06d664a49d369e1faf0782327b3ec            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:27:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 24 Oct 2022 21:27:22 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Mon, 24 Oct 2022 21:27:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 24 Oct 2022 21:27:23 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 24 Oct 2022 21:27:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 24 Oct 2022 21:27:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Mon, 24 Oct 2022 21:27:24 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Mon, 24 Oct 2022 21:27:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Oct 2022 21:27:25 GMT
CMD ["couchbase-server"]
# Mon, 24 Oct 2022 21:27:25 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 24 Oct 2022 21:27:25 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f6521e7788616a3d54de1df237a477200baa4fcdcbc80f1ca20102c8dac9a2`  
		Last Modified: Wed, 05 Oct 2022 16:52:36 GMT  
		Size: 6.2 MB (6232202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed4294155157022063832d043e5870cf3f0041b257eb6d0591a71ccb884e1ad`  
		Last Modified: Mon, 24 Oct 2022 21:29:40 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b75350ea80943a6d0b728ac523d24812c072e9df29e1b3dc9245795be253cdd`  
		Last Modified: Mon, 24 Oct 2022 21:30:37 GMT  
		Size: 565.2 MB (565241194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83fd8b65df9e1924726130bc71fd564d349c9362c18c537a875332b7868199e`  
		Last Modified: Mon, 24 Oct 2022 21:29:40 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a99cbee36c8d0b15280d3e06198929d60faa79e9b8c68d8eeb0a3876496659e`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 744.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa185d8f3874bc3626d0f50eb0c3a5807922e71c9df2f2c80dcb396fd02f6d4`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1041a169a865e16423286b77033d7444428e6accaf344bbaa08ee980294ddb4d`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d34e150d092d28dd1b92731f930fe34902f1007e6d3b5281bffdd8f401de39`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53731c36206040583c501d6cafb21deff20d807630c1eec787c7506843899a6f`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:7.1.2` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:fbdbeb909ed702aa4b1ae01e65338a169fa05e2c4c9ea2f8ee68707981de72ff
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.1 MB (574082024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5586e67f79257d6baa7d552a99933db1b205b6e626eb90e54a9b2458464284e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Mon, 24 Oct 2022 21:55:44 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 24 Oct 2022 21:55:44 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Mon, 24 Oct 2022 21:55:44 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:56:22 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Mon, 24 Oct 2022 21:56:22 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2
# Mon, 24 Oct 2022 21:56:23 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb
# Mon, 24 Oct 2022 21:56:23 GMT
ARG CB_SKIP_CHECKSUM=false
# Mon, 24 Oct 2022 21:56:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 24 Oct 2022 21:56:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 24 Oct 2022 21:57:20 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=1c7c757cf8aee87b98c96ffea1c26f4c98b6e0c053d966c8e760224030d98477            ;;          'amd64')            CB_SHA256=26fd9ae8585e0ea6637d4f1b492ed637dcf06d664a49d369e1faf0782327b3ec            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:57:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 24 Oct 2022 21:57:29 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Mon, 24 Oct 2022 21:57:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 24 Oct 2022 21:57:30 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 24 Oct 2022 21:57:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 24 Oct 2022 21:57:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Mon, 24 Oct 2022 21:57:31 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Mon, 24 Oct 2022 21:57:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Oct 2022 21:57:31 GMT
CMD ["couchbase-server"]
# Mon, 24 Oct 2022 21:57:31 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 24 Oct 2022 21:57:31 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd4213541647e0bd157630575f1ce12ab34bf86ddb1f38275d007ddee3c42e3`  
		Last Modified: Mon, 24 Oct 2022 21:58:32 GMT  
		Size: 6.1 MB (6058434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bf2e4f8352f457f4e17cefdb0a853638baf4f56e1918c045ddec2b1665ab2f`  
		Last Modified: Mon, 24 Oct 2022 21:58:31 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2b3271e89db387353725884822dba008cc472d29ce0fec112cfd2078a7100c`  
		Last Modified: Mon, 24 Oct 2022 21:59:11 GMT  
		Size: 540.8 MB (540827599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08a5945a886b16aedbd5dd6ae9b23996713053bf098818f205afea19881dbec`  
		Last Modified: Mon, 24 Oct 2022 21:58:31 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950b15f3a20c220dbcd3618f3772fd0bbdf7de89c7c3fb50627640a67bd1dff5`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 740.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727cf7782ced5c81cc91ffb1f9fb51766c5c2020061c14c87b2d3d8a12bf5c8d`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35449a251c18f484ccc31aedcb342ed8debd2e68abad0df55fed778de335c5fa`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36decd7e85da0aaf07f59bb9bc5f5dbe4d8924e028ba94e924b9199496c1b2cd`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c55cf5bd60c9cb4080ffb3224f22f72f7acf4bffefb903590a1f7b3e41977c`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community`

```console
$ docker pull couchbase@sha256:df6b5a560f9b4ec3dabea4fd32f4681aa37cd17af0c2f77399c845a17680e3d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:community` - linux; amd64

```console
$ docker pull couchbase@sha256:a1641cbf2ca8909c29a3b4e8da1170e53c456905ea03c3f478eb3f715fe544c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.6 MB (346610124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac174ce140cc2866a52eb39c1e35cf31772112a53d7252a546f2bc61a772e934`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:43:58 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 05 Oct 2022 16:43:58 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 05 Oct 2022 16:43:58 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 05 Oct 2022 16:44:32 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 05 Oct 2022 16:44:32 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1
# Wed, 05 Oct 2022 16:45:51 GMT
ARG CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb
# Wed, 05 Oct 2022 16:45:51 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 05 Oct 2022 16:45:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 05 Oct 2022 16:45:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 05 Oct 2022 16:46:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=275a0bb41d81920e9948fc05f736eef753179f698a04609eb8fe617d0fe55b8b            ;;          'amd64')            CB_SHA256=2fa47dc00f6d85aad5298149bb52450cc98c2c1e18eb54ab8ed45346c24a9403            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 05 Oct 2022 16:46:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 05 Oct 2022 16:46:34 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 05 Oct 2022 16:46:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 05 Oct 2022 16:46:35 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 05 Oct 2022 16:46:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 05 Oct 2022 16:46:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 05 Oct 2022 16:46:36 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 05 Oct 2022 16:46:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 16:46:36 GMT
CMD ["couchbase-server"]
# Wed, 05 Oct 2022 16:46:36 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 05 Oct 2022 16:46:36 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f6521e7788616a3d54de1df237a477200baa4fcdcbc80f1ca20102c8dac9a2`  
		Last Modified: Wed, 05 Oct 2022 16:52:36 GMT  
		Size: 6.2 MB (6232202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a76af002daa40f0ed977962becd577d570ddfdb52cb9fbbee8820b5026ddd9b`  
		Last Modified: Wed, 05 Oct 2022 16:53:49 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7e2fa750d6086b108755383968f5702808faa7331e6fe8dabe30a47c61d034`  
		Last Modified: Wed, 05 Oct 2022 16:54:27 GMT  
		Size: 311.8 MB (311799111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ba95fd25d37825cef50ccd4351bfe5243f6ad5ea3ac0b231434b3b5727950d`  
		Last Modified: Wed, 05 Oct 2022 16:53:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea5a3d3d340b7832dabf925f161e94224c1a7861e02b65de865aa7a1b548c0c`  
		Last Modified: Wed, 05 Oct 2022 16:53:47 GMT  
		Size: 740.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbe635bf4fa22c67d409b1a9e9c49f46f907158ee2ced1088d1f87716536114`  
		Last Modified: Wed, 05 Oct 2022 16:53:47 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9306f14959fea72c77d7f38b7b78d863eeb36737c0171cc1ac0528b2441e6b30`  
		Last Modified: Wed, 05 Oct 2022 16:53:47 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0f8d4e53852f13bf5ab8eb1ef0426fdd5f32eec514b2e67bdd53681b3b085a`  
		Last Modified: Wed, 05 Oct 2022 16:53:47 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22834a75d47024bc9a12562f81b305c33230b726d1de7a1ae47a6af60af1c01c`  
		Last Modified: Wed, 05 Oct 2022 16:53:47 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:community` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:5f95401144746c9c62b2cb735bc03aab70a705edac98c85899586d6b3ae40ac2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.3 MB (327280228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a248d00b3b4235263607d8336652b6dbd4facff4930864d1b0e686ae45523068`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Mon, 24 Oct 2022 21:55:44 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 24 Oct 2022 21:55:44 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Mon, 24 Oct 2022 21:55:44 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:56:22 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Mon, 24 Oct 2022 21:57:37 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1
# Mon, 24 Oct 2022 21:57:37 GMT
ARG CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb
# Mon, 24 Oct 2022 21:57:37 GMT
ARG CB_SKIP_CHECKSUM=false
# Mon, 24 Oct 2022 21:57:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 24 Oct 2022 21:57:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 24 Oct 2022 21:58:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=275a0bb41d81920e9948fc05f736eef753179f698a04609eb8fe617d0fe55b8b            ;;          'amd64')            CB_SHA256=2fa47dc00f6d85aad5298149bb52450cc98c2c1e18eb54ab8ed45346c24a9403            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:58:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 24 Oct 2022 21:58:08 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Mon, 24 Oct 2022 21:58:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 24 Oct 2022 21:58:08 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 24 Oct 2022 21:58:09 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 24 Oct 2022 21:58:09 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Mon, 24 Oct 2022 21:58:09 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Mon, 24 Oct 2022 21:58:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Oct 2022 21:58:09 GMT
CMD ["couchbase-server"]
# Mon, 24 Oct 2022 21:58:09 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 24 Oct 2022 21:58:10 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd4213541647e0bd157630575f1ce12ab34bf86ddb1f38275d007ddee3c42e3`  
		Last Modified: Mon, 24 Oct 2022 21:58:32 GMT  
		Size: 6.1 MB (6058434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0242a785a71d2df50336c954a2970e24aef1eaef860cf7330e689407a08eb081`  
		Last Modified: Mon, 24 Oct 2022 21:59:28 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:029e62a87155047dd3b850efb90988f270f457ba3a7941a6560161035d85a7dc`  
		Last Modified: Mon, 24 Oct 2022 21:59:55 GMT  
		Size: 294.0 MB (294025812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9aa76649c6f09c7360cb85118ef10568e2703a61476ab300053be341ec23e5`  
		Last Modified: Mon, 24 Oct 2022 21:59:28 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d861f940fa67e7a7f85c7b0fe27c15ad2fec7fa1f7b41ffd3e65936143293df1`  
		Last Modified: Mon, 24 Oct 2022 21:59:26 GMT  
		Size: 739.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cf18e5f46f085339325b46627744de26c4eedd3d92b6807b8df656d024ca2a`  
		Last Modified: Mon, 24 Oct 2022 21:59:26 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad1edc88f4e16c6807804ece824ad9b3e0d9c92a93d7c8b3c27cd5e3cb7e1c3`  
		Last Modified: Mon, 24 Oct 2022 21:59:26 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd6266df51ff1f30670947e44fc6642b05c79a30241bb2363a3635615575b68`  
		Last Modified: Mon, 24 Oct 2022 21:59:26 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a989dc2d337e9d6ad02fb476e75c0496a5a9e877e12d30e401e37bd6a20835`  
		Last Modified: Mon, 24 Oct 2022 21:59:26 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-6.6.0`

```console
$ docker pull couchbase@sha256:4fc1b5b450de7ad1b4549b8cb516adfcd48a2ac1e7e2ac1711d1edc90e2455df
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-6.6.0` - linux; amd64

```console
$ docker pull couchbase@sha256:4f593ec70db07613d77b095a787600432ef610fcdade5345c2837b1acc35be47
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.5 MB (352538865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a57aa7e6dee8b500915dfd8f6f0f6f31eb4d4cbf37376364d1d015c017431d61`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:04 GMT
ADD file:ed601c56cf74241eeb1971b24ed969fb855cd2b9330276d3c5779ecdb0b28364 in / 
# Tue, 04 Oct 2022 23:35:04 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:50:36 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 05 Oct 2022 16:50:36 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 05 Oct 2022 16:50:37 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 05 Oct 2022 16:50:55 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 05 Oct 2022 16:50:55 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Wed, 05 Oct 2022 16:50:55 GMT
ARG CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb
# Wed, 05 Oct 2022 16:50:55 GMT
ARG CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559
# Wed, 05 Oct 2022 16:50:55 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 05 Oct 2022 16:50:55 GMT
ARG CB_PACKAGE_NAME=couchbase-server-community
# Wed, 05 Oct 2022 16:50:55 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 05 Oct 2022 16:50:56 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 05 Oct 2022 16:51:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && dpkg --unpack ./$CB_PACKAGE     && sed -i -e '/Best heuristic/ a \ \ \ \ [ -d /run/systemd/system ] && return 1; return 0' /opt/couchbase/bin/install/systemd-ctl     && dpkg --configure couchbase-server-community     && apt-get install -yf     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 05 Oct 2022 16:51:51 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 05 Oct 2022 16:51:51 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 05 Oct 2022 16:51:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 05 Oct 2022 16:51:52 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 05 Oct 2022 16:51:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 05 Oct 2022 16:52:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu18.04_amd64.deb CB_PACKAGE_NAME=couchbase-server-community CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9b196cd7be81d7d6b179838e9d30164fdb7a1f27e96678e61e24e9fe5c93f559 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 05 Oct 2022 16:52:01 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 05 Oct 2022 16:52:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 16:52:01 GMT
CMD ["couchbase-server"]
# Wed, 05 Oct 2022 16:52:01 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 05 Oct 2022 16:52:01 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:e706e0a9f42365312b366bf4caa22f3cdd8fc7fd8f6f49b4dd3782711f66aca7`  
		Last Modified: Tue, 04 Oct 2022 11:37:26 GMT  
		Size: 26.7 MB (26711852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a57358449e1d424e033ab8a75537ee0c57e17f1b75e4071a5108d41d9f7f7b`  
		Last Modified: Wed, 05 Oct 2022 16:58:04 GMT  
		Size: 5.6 MB (5626012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ece7c18d91bad051976e13438369f8c260ae66c52ff87e7e3bc3dd2fac1460`  
		Last Modified: Wed, 05 Oct 2022 16:58:02 GMT  
		Size: 2.0 KB (1966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7715c73f5a01fca5abebdf6d81ad85b2a31d3bab3555d04b813658bdbf88817e`  
		Last Modified: Wed, 05 Oct 2022 16:58:37 GMT  
		Size: 319.8 MB (319763132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b6344d327858a08151f39d897281078e830c07377e6088cd8423da504f1c665`  
		Last Modified: Wed, 05 Oct 2022 16:58:02 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c33fa52ee45962c7330074f1ccb141f5f8cf72a1380a151b6883e2e1ad7a263`  
		Last Modified: Wed, 05 Oct 2022 16:58:02 GMT  
		Size: 741.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9af063723658d50e93af921641500dc599c109ca3c1e3b044b01d13f09e41ced`  
		Last Modified: Wed, 05 Oct 2022 16:58:00 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e62c41534bb85ff8a0d9e7e1122363f4ebfb335a11628f0934e6cb1bf7bc05`  
		Last Modified: Wed, 05 Oct 2022 16:58:00 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291064e2c505e802cd4f6f43fd83c50ebd6babf6a35c04e7f64c90e3455224d3`  
		Last Modified: Wed, 05 Oct 2022 16:58:00 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6a29ca60bd925c70d89da9482448abfa6f71e1cecc74d6297ae5af2ee847a0`  
		Last Modified: Wed, 05 Oct 2022 16:58:00 GMT  
		Size: 433.4 KB (433373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdaf5dc0c1855b6363c75d3fd5dc61e06d448a57cea7c477d3961e543378b421`  
		Last Modified: Wed, 05 Oct 2022 16:58:00 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-7.0.2`

```console
$ docker pull couchbase@sha256:e065bea7b05ee301b39903d1f0c31e54ca30f70492ca08e1e1244d0e152f6e18
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:community-7.0.2` - linux; amd64

```console
$ docker pull couchbase@sha256:1f3a0de6c119e638f6f15efdd01b130f943f373832b0093fc3eb7b386462abab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **429.0 MB (429011279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a60f792fb7e57184554f14bc4edc2b7fd328858cd07490dba15e9e328a1a222a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:43:58 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 05 Oct 2022 16:48:27 GMT
RUN set -x &&     apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 05 Oct 2022 16:48:28 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 05 Oct 2022 16:48:28 GMT
ARG CB_VERSION=7.0.2
# Wed, 05 Oct 2022 16:48:28 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2
# Wed, 05 Oct 2022 16:48:28 GMT
ARG CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb
# Wed, 05 Oct 2022 16:48:28 GMT
ARG CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e
# Wed, 05 Oct 2022 16:48:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 05 Oct 2022 16:48:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 05 Oct 2022 16:49:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN set -x &&     export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     apt-get update &&     apt-get install -y ./$CB_PACKAGE &&     rm -f ./$CB_PACKAGE &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 05 Oct 2022 16:49:21 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 05 Oct 2022 16:49:21 GMT
COPY file:cf9c7c8a9eda8a5fefcaa60d67181024b8a07b30eb318d4c9591b33a95ca6680 in /etc/service/couchbase-server/run 
# Wed, 05 Oct 2022 16:49:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 05 Oct 2022 16:49:22 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 05 Oct 2022 16:49:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 05 Oct 2022 16:49:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.2-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.2 CB_SHA256=f935dcad5c04b553a3c56d782c8d9cb782cbd1cf88878a425ba5f9d45d08120e CB_VERSION=7.0.2
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 05 Oct 2022 16:49:23 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 05 Oct 2022 16:49:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 16:49:23 GMT
CMD ["couchbase-server"]
# Wed, 05 Oct 2022 16:49:23 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 05 Oct 2022 16:49:23 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a1bfe8ef9b2fc448defe5cc1dbb0128fc88b0f868393cfa07a31cf466953417`  
		Last Modified: Wed, 05 Oct 2022 16:56:03 GMT  
		Size: 6.2 MB (6240633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fe788f80bb0080f0d6e1932bce901001156e7374b8d8a42c14ff8d0951fb0a`  
		Last Modified: Wed, 05 Oct 2022 16:56:00 GMT  
		Size: 264.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ed2677f2df697f6ec59ff59d5e02776f0861829161bd35d8161083ba118899`  
		Last Modified: Wed, 05 Oct 2022 16:56:00 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4cc06d4292a449d99efd2cc107bfd070df3266d06205dcbd1b645f2e344466`  
		Last Modified: Wed, 05 Oct 2022 16:56:47 GMT  
		Size: 394.1 MB (394062203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b90a5f1b58a0d5701bf4ea3af14a14ac845b414f2394ef98d8431cb92c37d278`  
		Last Modified: Wed, 05 Oct 2022 16:56:00 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160829ff7139964fba8830b085141397deb102e5d0fdb5048d49bfc566b5f963`  
		Last Modified: Wed, 05 Oct 2022 16:56:00 GMT  
		Size: 603.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b040ddb7b11a04738b2ab2f63e712fbe7959b8de840f25f374b23b6d566f66`  
		Last Modified: Wed, 05 Oct 2022 16:55:58 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8a366e1a7f44de3c1fcbd9370034f268e9ffa7370d34a2eb87b5fbc3167ff6`  
		Last Modified: Wed, 05 Oct 2022 16:55:58 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8d78f571d7fd93e28dd563eed69cc7d7ca8e900ec87099e696e346896d16ed`  
		Last Modified: Wed, 05 Oct 2022 16:55:58 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962a0c71a11fc31a0645d180b0bcd4fc172b665ec75dda999bf9fc5537a9da84`  
		Last Modified: Wed, 05 Oct 2022 16:55:58 GMT  
		Size: 129.5 KB (129510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc2f3030821770f26f7bc81b8b1e9df0b5d6757e117bf2d3b65f50eceea364c`  
		Last Modified: Wed, 05 Oct 2022 16:55:58 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-7.1.1`

```console
$ docker pull couchbase@sha256:df6b5a560f9b4ec3dabea4fd32f4681aa37cd17af0c2f77399c845a17680e3d7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:community-7.1.1` - linux; amd64

```console
$ docker pull couchbase@sha256:a1641cbf2ca8909c29a3b4e8da1170e53c456905ea03c3f478eb3f715fe544c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **346.6 MB (346610124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac174ce140cc2866a52eb39c1e35cf31772112a53d7252a546f2bc61a772e934`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:43:58 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 05 Oct 2022 16:43:58 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 05 Oct 2022 16:43:58 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 05 Oct 2022 16:44:32 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 05 Oct 2022 16:44:32 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1
# Wed, 05 Oct 2022 16:45:51 GMT
ARG CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb
# Wed, 05 Oct 2022 16:45:51 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 05 Oct 2022 16:45:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 05 Oct 2022 16:45:52 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 05 Oct 2022 16:46:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=275a0bb41d81920e9948fc05f736eef753179f698a04609eb8fe617d0fe55b8b            ;;          'amd64')            CB_SHA256=2fa47dc00f6d85aad5298149bb52450cc98c2c1e18eb54ab8ed45346c24a9403            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 05 Oct 2022 16:46:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 05 Oct 2022 16:46:34 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 05 Oct 2022 16:46:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 05 Oct 2022 16:46:35 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 05 Oct 2022 16:46:35 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 05 Oct 2022 16:46:36 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 05 Oct 2022 16:46:36 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 05 Oct 2022 16:46:36 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 16:46:36 GMT
CMD ["couchbase-server"]
# Wed, 05 Oct 2022 16:46:36 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 05 Oct 2022 16:46:36 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f6521e7788616a3d54de1df237a477200baa4fcdcbc80f1ca20102c8dac9a2`  
		Last Modified: Wed, 05 Oct 2022 16:52:36 GMT  
		Size: 6.2 MB (6232202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a76af002daa40f0ed977962becd577d570ddfdb52cb9fbbee8820b5026ddd9b`  
		Last Modified: Wed, 05 Oct 2022 16:53:49 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca7e2fa750d6086b108755383968f5702808faa7331e6fe8dabe30a47c61d034`  
		Last Modified: Wed, 05 Oct 2022 16:54:27 GMT  
		Size: 311.8 MB (311799111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ba95fd25d37825cef50ccd4351bfe5243f6ad5ea3ac0b231434b3b5727950d`  
		Last Modified: Wed, 05 Oct 2022 16:53:49 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ea5a3d3d340b7832dabf925f161e94224c1a7861e02b65de865aa7a1b548c0c`  
		Last Modified: Wed, 05 Oct 2022 16:53:47 GMT  
		Size: 740.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbe635bf4fa22c67d409b1a9e9c49f46f907158ee2ced1088d1f87716536114`  
		Last Modified: Wed, 05 Oct 2022 16:53:47 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9306f14959fea72c77d7f38b7b78d863eeb36737c0171cc1ac0528b2441e6b30`  
		Last Modified: Wed, 05 Oct 2022 16:53:47 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef0f8d4e53852f13bf5ab8eb1ef0426fdd5f32eec514b2e67bdd53681b3b085a`  
		Last Modified: Wed, 05 Oct 2022 16:53:47 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22834a75d47024bc9a12562f81b305c33230b726d1de7a1ae47a6af60af1c01c`  
		Last Modified: Wed, 05 Oct 2022 16:53:47 GMT  
		Size: 867.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:community-7.1.1` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:5f95401144746c9c62b2cb735bc03aab70a705edac98c85899586d6b3ae40ac2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.3 MB (327280228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a248d00b3b4235263607d8336652b6dbd4facff4930864d1b0e686ae45523068`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Mon, 24 Oct 2022 21:55:44 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 24 Oct 2022 21:55:44 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Mon, 24 Oct 2022 21:55:44 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:56:22 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Mon, 24 Oct 2022 21:57:37 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1
# Mon, 24 Oct 2022 21:57:37 GMT
ARG CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb
# Mon, 24 Oct 2022 21:57:37 GMT
ARG CB_SKIP_CHECKSUM=false
# Mon, 24 Oct 2022 21:57:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 24 Oct 2022 21:57:37 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 24 Oct 2022 21:58:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=275a0bb41d81920e9948fc05f736eef753179f698a04609eb8fe617d0fe55b8b            ;;          'amd64')            CB_SHA256=2fa47dc00f6d85aad5298149bb52450cc98c2c1e18eb54ab8ed45346c24a9403            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:58:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 24 Oct 2022 21:58:08 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Mon, 24 Oct 2022 21:58:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 24 Oct 2022 21:58:08 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 24 Oct 2022 21:58:09 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 24 Oct 2022 21:58:09 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Mon, 24 Oct 2022 21:58:09 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Mon, 24 Oct 2022 21:58:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Oct 2022 21:58:09 GMT
CMD ["couchbase-server"]
# Mon, 24 Oct 2022 21:58:09 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 24 Oct 2022 21:58:10 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd4213541647e0bd157630575f1ce12ab34bf86ddb1f38275d007ddee3c42e3`  
		Last Modified: Mon, 24 Oct 2022 21:58:32 GMT  
		Size: 6.1 MB (6058434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0242a785a71d2df50336c954a2970e24aef1eaef860cf7330e689407a08eb081`  
		Last Modified: Mon, 24 Oct 2022 21:59:28 GMT  
		Size: 1.8 KB (1836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:029e62a87155047dd3b850efb90988f270f457ba3a7941a6560161035d85a7dc`  
		Last Modified: Mon, 24 Oct 2022 21:59:55 GMT  
		Size: 294.0 MB (294025812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e9aa76649c6f09c7360cb85118ef10568e2703a61476ab300053be341ec23e5`  
		Last Modified: Mon, 24 Oct 2022 21:59:28 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d861f940fa67e7a7f85c7b0fe27c15ad2fec7fa1f7b41ffd3e65936143293df1`  
		Last Modified: Mon, 24 Oct 2022 21:59:26 GMT  
		Size: 739.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9cf18e5f46f085339325b46627744de26c4eedd3d92b6807b8df656d024ca2a`  
		Last Modified: Mon, 24 Oct 2022 21:59:26 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad1edc88f4e16c6807804ece824ad9b3e0d9c92a93d7c8b3c27cd5e3cb7e1c3`  
		Last Modified: Mon, 24 Oct 2022 21:59:26 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dd6266df51ff1f30670947e44fc6642b05c79a30241bb2363a3635615575b68`  
		Last Modified: Mon, 24 Oct 2022 21:59:26 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72a989dc2d337e9d6ad02fb476e75c0496a5a9e877e12d30e401e37bd6a20835`  
		Last Modified: Mon, 24 Oct 2022 21:59:26 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise`

```console
$ docker pull couchbase@sha256:fb14ff77878dcc2f53b40764d8b7413268026a3a52d04ed3a06fede454e64d8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:enterprise` - linux; amd64

```console
$ docker pull couchbase@sha256:43db9f11908feafb47719a0e926bfb3875efa4eb34bf233856b7e3a75778c2e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **600.1 MB (600052223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a4e33350b160e36ed40a8ffe8424cfb308dad94279fa3e50445693d7666352`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:43:58 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 05 Oct 2022 16:43:58 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 05 Oct 2022 16:43:58 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 05 Oct 2022 16:44:32 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Mon, 24 Oct 2022 21:25:59 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2
# Mon, 24 Oct 2022 21:25:59 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb
# Mon, 24 Oct 2022 21:25:59 GMT
ARG CB_SKIP_CHECKSUM=false
# Mon, 24 Oct 2022 21:25:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 24 Oct 2022 21:26:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 24 Oct 2022 21:27:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=1c7c757cf8aee87b98c96ffea1c26f4c98b6e0c053d966c8e760224030d98477            ;;          'amd64')            CB_SHA256=26fd9ae8585e0ea6637d4f1b492ed637dcf06d664a49d369e1faf0782327b3ec            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:27:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 24 Oct 2022 21:27:22 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Mon, 24 Oct 2022 21:27:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 24 Oct 2022 21:27:23 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 24 Oct 2022 21:27:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 24 Oct 2022 21:27:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Mon, 24 Oct 2022 21:27:24 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Mon, 24 Oct 2022 21:27:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Oct 2022 21:27:25 GMT
CMD ["couchbase-server"]
# Mon, 24 Oct 2022 21:27:25 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 24 Oct 2022 21:27:25 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f6521e7788616a3d54de1df237a477200baa4fcdcbc80f1ca20102c8dac9a2`  
		Last Modified: Wed, 05 Oct 2022 16:52:36 GMT  
		Size: 6.2 MB (6232202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed4294155157022063832d043e5870cf3f0041b257eb6d0591a71ccb884e1ad`  
		Last Modified: Mon, 24 Oct 2022 21:29:40 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b75350ea80943a6d0b728ac523d24812c072e9df29e1b3dc9245795be253cdd`  
		Last Modified: Mon, 24 Oct 2022 21:30:37 GMT  
		Size: 565.2 MB (565241194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83fd8b65df9e1924726130bc71fd564d349c9362c18c537a875332b7868199e`  
		Last Modified: Mon, 24 Oct 2022 21:29:40 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a99cbee36c8d0b15280d3e06198929d60faa79e9b8c68d8eeb0a3876496659e`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 744.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa185d8f3874bc3626d0f50eb0c3a5807922e71c9df2f2c80dcb396fd02f6d4`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1041a169a865e16423286b77033d7444428e6accaf344bbaa08ee980294ddb4d`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d34e150d092d28dd1b92731f930fe34902f1007e6d3b5281bffdd8f401de39`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53731c36206040583c501d6cafb21deff20d807630c1eec787c7506843899a6f`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:enterprise` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:fbdbeb909ed702aa4b1ae01e65338a169fa05e2c4c9ea2f8ee68707981de72ff
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.1 MB (574082024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5586e67f79257d6baa7d552a99933db1b205b6e626eb90e54a9b2458464284e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Mon, 24 Oct 2022 21:55:44 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 24 Oct 2022 21:55:44 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Mon, 24 Oct 2022 21:55:44 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:56:22 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Mon, 24 Oct 2022 21:56:22 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2
# Mon, 24 Oct 2022 21:56:23 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb
# Mon, 24 Oct 2022 21:56:23 GMT
ARG CB_SKIP_CHECKSUM=false
# Mon, 24 Oct 2022 21:56:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 24 Oct 2022 21:56:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 24 Oct 2022 21:57:20 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=1c7c757cf8aee87b98c96ffea1c26f4c98b6e0c053d966c8e760224030d98477            ;;          'amd64')            CB_SHA256=26fd9ae8585e0ea6637d4f1b492ed637dcf06d664a49d369e1faf0782327b3ec            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:57:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 24 Oct 2022 21:57:29 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Mon, 24 Oct 2022 21:57:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 24 Oct 2022 21:57:30 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 24 Oct 2022 21:57:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 24 Oct 2022 21:57:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Mon, 24 Oct 2022 21:57:31 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Mon, 24 Oct 2022 21:57:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Oct 2022 21:57:31 GMT
CMD ["couchbase-server"]
# Mon, 24 Oct 2022 21:57:31 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 24 Oct 2022 21:57:31 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd4213541647e0bd157630575f1ce12ab34bf86ddb1f38275d007ddee3c42e3`  
		Last Modified: Mon, 24 Oct 2022 21:58:32 GMT  
		Size: 6.1 MB (6058434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bf2e4f8352f457f4e17cefdb0a853638baf4f56e1918c045ddec2b1665ab2f`  
		Last Modified: Mon, 24 Oct 2022 21:58:31 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2b3271e89db387353725884822dba008cc472d29ce0fec112cfd2078a7100c`  
		Last Modified: Mon, 24 Oct 2022 21:59:11 GMT  
		Size: 540.8 MB (540827599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08a5945a886b16aedbd5dd6ae9b23996713053bf098818f205afea19881dbec`  
		Last Modified: Mon, 24 Oct 2022 21:58:31 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950b15f3a20c220dbcd3618f3772fd0bbdf7de89c7c3fb50627640a67bd1dff5`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 740.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727cf7782ced5c81cc91ffb1f9fb51766c5c2020061c14c87b2d3d8a12bf5c8d`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35449a251c18f484ccc31aedcb342ed8debd2e68abad0df55fed778de335c5fa`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36decd7e85da0aaf07f59bb9bc5f5dbe4d8924e028ba94e924b9199496c1b2cd`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c55cf5bd60c9cb4080ffb3224f22f72f7acf4bffefb903590a1f7b3e41977c`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.6.5`

```console
$ docker pull couchbase@sha256:f1ed8218ba5b59fb643e32966f9e834cd8cf969c571e16a64e3bf397a3ae4394
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-6.6.5` - linux; amd64

```console
$ docker pull couchbase@sha256:e5cc2084694132e099f7640c314f52e8733bcad173b2553ebb5342123053305d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **540.9 MB (540902425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1b16ba5ebc72018eb36e6dd59cd9d20f78d7686b96869002e952c0026308f74`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:43:58 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 05 Oct 2022 16:43:58 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 05 Oct 2022 16:43:58 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 05 Oct 2022 16:44:32 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 05 Oct 2022 16:49:27 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5
# Wed, 05 Oct 2022 16:49:27 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb
# Wed, 05 Oct 2022 16:49:27 GMT
ARG CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6
# Wed, 05 Oct 2022 16:49:27 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 05 Oct 2022 16:49:27 GMT
ARG CB_PACKAGE_NAME=couchbase-server
# Wed, 05 Oct 2022 16:49:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 05 Oct 2022 16:49:28 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 05 Oct 2022 16:50:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && dpkg --unpack ./$CB_PACKAGE     && sed -i -e '/Best heuristic/ a \ \ \ \ [ -d /run/systemd/system ] && return 1; return 0' /opt/couchbase/bin/install/systemd-ctl     && dpkg --configure couchbase-server     && apt-get install -yf     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 05 Oct 2022 16:50:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 05 Oct 2022 16:50:23 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 05 Oct 2022 16:50:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 05 Oct 2022 16:50:24 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 05 Oct 2022 16:50:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 05 Oct 2022 16:50:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.5-ubuntu20.04_amd64.deb CB_PACKAGE_NAME=couchbase-server CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.5 CB_SHA256=fb2da1880ea993dc7a5695c6fbe14cde62024d865a71a7d44ab653f0f633d4c6 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 05 Oct 2022 16:50:31 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 05 Oct 2022 16:50:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 16:50:31 GMT
CMD ["couchbase-server"]
# Wed, 05 Oct 2022 16:50:31 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 05 Oct 2022 16:50:32 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f6521e7788616a3d54de1df237a477200baa4fcdcbc80f1ca20102c8dac9a2`  
		Last Modified: Wed, 05 Oct 2022 16:52:36 GMT  
		Size: 6.2 MB (6232202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18dd9c54682a90764bcd4ab2ea200d80fccb8d87501195e6611a9b6b410f6505`  
		Last Modified: Wed, 05 Oct 2022 16:56:56 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5affd3fa6a36992a447da553db74ba262aea2c14198d0c1d470b8b6eab16d888`  
		Last Modified: Wed, 05 Oct 2022 16:57:49 GMT  
		Size: 505.7 MB (505651775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c10c297192bd86a2c0f056b6ac8204ef405238d034f694279475f66e53967be9`  
		Last Modified: Wed, 05 Oct 2022 16:56:56 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8f4ec6103f66664911ae3c569a7c49c826f0563488b7b6c35d36a7a5609deb`  
		Last Modified: Wed, 05 Oct 2022 16:56:56 GMT  
		Size: 738.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e3bce98c83822f6ee9604fc88a7b4bfe84d64c7cf771396f8b9d6bed7cf413`  
		Last Modified: Wed, 05 Oct 2022 16:56:54 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8788b0f02f82a694f4d429b38c3823e038f77b4ffd60aa97bcdc94a89cd9b372`  
		Last Modified: Wed, 05 Oct 2022 16:56:54 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6def2a48c9d2562a5bf5b839a8f640634a75413dd351ae7323d0c7c9a94a093`  
		Last Modified: Wed, 05 Oct 2022 16:56:54 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4323301d29d5923422b1f072ff6a1338ba9f893c9226a19e0a1b03d2c13ea540`  
		Last Modified: Wed, 05 Oct 2022 16:56:55 GMT  
		Size: 439.6 KB (439628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262160f2dba6a58a826580627d7887a70a0ad12d71b1b05842f0f5747231035d`  
		Last Modified: Wed, 05 Oct 2022 16:56:54 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-7.0.4`

```console
$ docker pull couchbase@sha256:6fb17f745b5d12f7986b1f71092210e186b836ac6d1f29158288d681d2473154
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-7.0.4` - linux; amd64

```console
$ docker pull couchbase@sha256:bb6b822e4a36e770aedf2c084e3872fd3088591e51891fdf33c79dca344e2f1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **641.1 MB (641145367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61698097571dc39f0348f6088aad6ff50d956002bd50643ec71d558e422189a6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:43:58 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 05 Oct 2022 16:43:58 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 05 Oct 2022 16:43:58 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 05 Oct 2022 16:44:32 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Mon, 24 Oct 2022 21:27:39 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4
# Mon, 24 Oct 2022 21:27:39 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb
# Mon, 24 Oct 2022 21:27:39 GMT
ARG CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2
# Mon, 24 Oct 2022 21:27:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 24 Oct 2022 21:27:40 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4 CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 24 Oct 2022 21:28:50 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4 CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c -     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:28:55 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4 CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 24 Oct 2022 21:28:55 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Mon, 24 Oct 2022 21:28:56 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4 CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 24 Oct 2022 21:28:56 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 24 Oct 2022 21:28:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4 CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 24 Oct 2022 21:29:04 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.4-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.4 CB_SHA256=dfa3c2eec3cbf31ee200eb1423f4b19719edd0b73fdf1132956302462b74a9b2 CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Mon, 24 Oct 2022 21:29:05 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Mon, 24 Oct 2022 21:29:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Oct 2022 21:29:05 GMT
CMD ["couchbase-server"]
# Mon, 24 Oct 2022 21:29:05 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 24 Oct 2022 21:29:05 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f6521e7788616a3d54de1df237a477200baa4fcdcbc80f1ca20102c8dac9a2`  
		Last Modified: Wed, 05 Oct 2022 16:52:36 GMT  
		Size: 6.2 MB (6232202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecab90dac59c107f5dd70235be20f72b55b47b158f63b47125d6c0fd191ca930`  
		Last Modified: Mon, 24 Oct 2022 21:30:57 GMT  
		Size: 1.8 KB (1845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd53ad08efa52facea1982c7bdc350701fbf18f07001d6473ff093e2964d3be`  
		Last Modified: Mon, 24 Oct 2022 21:32:30 GMT  
		Size: 605.9 MB (605890340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3df565d7527eb8d41cd1662a1635d93b007ec3384e31eaa21b8cf26304206a5d`  
		Last Modified: Mon, 24 Oct 2022 21:30:57 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b846649aa7e9275d1385f3ac587ced227eb211415c82da98d27118a8f46b29`  
		Last Modified: Mon, 24 Oct 2022 21:30:57 GMT  
		Size: 744.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d227861109fc824e1e97687726cdf9ef1d92b5a0d6c27e8e0c61be9fce5261`  
		Last Modified: Mon, 24 Oct 2022 21:30:55 GMT  
		Size: 282.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68bc438f6eaf8ccd9d706a6400206b43a40ffe96eefb61dd25f74183d435a8f2`  
		Last Modified: Mon, 24 Oct 2022 21:30:55 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646ea57d4f974ef19e4e88ae9745b730a3c3cb2cc75a304474c66d0ad871022e`  
		Last Modified: Mon, 24 Oct 2022 21:30:55 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a8989065f3279985c667aaa8eb0ec3420dc0db82c225e04dade8238dd9459d`  
		Last Modified: Mon, 24 Oct 2022 21:30:55 GMT  
		Size: 444.0 KB (443988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59389ff2f8c5cfc0bf8b97dce5b001f6f2bb88230bfb119146071c5144bba1c9`  
		Last Modified: Mon, 24 Oct 2022 21:30:55 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-7.1.2`

```console
$ docker pull couchbase@sha256:fb14ff77878dcc2f53b40764d8b7413268026a3a52d04ed3a06fede454e64d8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:enterprise-7.1.2` - linux; amd64

```console
$ docker pull couchbase@sha256:43db9f11908feafb47719a0e926bfb3875efa4eb34bf233856b7e3a75778c2e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **600.1 MB (600052223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a4e33350b160e36ed40a8ffe8424cfb308dad94279fa3e50445693d7666352`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:43:58 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 05 Oct 2022 16:43:58 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 05 Oct 2022 16:43:58 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 05 Oct 2022 16:44:32 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Mon, 24 Oct 2022 21:25:59 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2
# Mon, 24 Oct 2022 21:25:59 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb
# Mon, 24 Oct 2022 21:25:59 GMT
ARG CB_SKIP_CHECKSUM=false
# Mon, 24 Oct 2022 21:25:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 24 Oct 2022 21:26:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 24 Oct 2022 21:27:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=1c7c757cf8aee87b98c96ffea1c26f4c98b6e0c053d966c8e760224030d98477            ;;          'amd64')            CB_SHA256=26fd9ae8585e0ea6637d4f1b492ed637dcf06d664a49d369e1faf0782327b3ec            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:27:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 24 Oct 2022 21:27:22 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Mon, 24 Oct 2022 21:27:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 24 Oct 2022 21:27:23 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 24 Oct 2022 21:27:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 24 Oct 2022 21:27:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Mon, 24 Oct 2022 21:27:24 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Mon, 24 Oct 2022 21:27:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Oct 2022 21:27:25 GMT
CMD ["couchbase-server"]
# Mon, 24 Oct 2022 21:27:25 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 24 Oct 2022 21:27:25 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f6521e7788616a3d54de1df237a477200baa4fcdcbc80f1ca20102c8dac9a2`  
		Last Modified: Wed, 05 Oct 2022 16:52:36 GMT  
		Size: 6.2 MB (6232202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed4294155157022063832d043e5870cf3f0041b257eb6d0591a71ccb884e1ad`  
		Last Modified: Mon, 24 Oct 2022 21:29:40 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b75350ea80943a6d0b728ac523d24812c072e9df29e1b3dc9245795be253cdd`  
		Last Modified: Mon, 24 Oct 2022 21:30:37 GMT  
		Size: 565.2 MB (565241194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83fd8b65df9e1924726130bc71fd564d349c9362c18c537a875332b7868199e`  
		Last Modified: Mon, 24 Oct 2022 21:29:40 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a99cbee36c8d0b15280d3e06198929d60faa79e9b8c68d8eeb0a3876496659e`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 744.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa185d8f3874bc3626d0f50eb0c3a5807922e71c9df2f2c80dcb396fd02f6d4`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1041a169a865e16423286b77033d7444428e6accaf344bbaa08ee980294ddb4d`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d34e150d092d28dd1b92731f930fe34902f1007e6d3b5281bffdd8f401de39`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53731c36206040583c501d6cafb21deff20d807630c1eec787c7506843899a6f`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:enterprise-7.1.2` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:fbdbeb909ed702aa4b1ae01e65338a169fa05e2c4c9ea2f8ee68707981de72ff
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.1 MB (574082024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5586e67f79257d6baa7d552a99933db1b205b6e626eb90e54a9b2458464284e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Mon, 24 Oct 2022 21:55:44 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 24 Oct 2022 21:55:44 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Mon, 24 Oct 2022 21:55:44 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:56:22 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Mon, 24 Oct 2022 21:56:22 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2
# Mon, 24 Oct 2022 21:56:23 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb
# Mon, 24 Oct 2022 21:56:23 GMT
ARG CB_SKIP_CHECKSUM=false
# Mon, 24 Oct 2022 21:56:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 24 Oct 2022 21:56:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 24 Oct 2022 21:57:20 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=1c7c757cf8aee87b98c96ffea1c26f4c98b6e0c053d966c8e760224030d98477            ;;          'amd64')            CB_SHA256=26fd9ae8585e0ea6637d4f1b492ed637dcf06d664a49d369e1faf0782327b3ec            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:57:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 24 Oct 2022 21:57:29 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Mon, 24 Oct 2022 21:57:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 24 Oct 2022 21:57:30 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 24 Oct 2022 21:57:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 24 Oct 2022 21:57:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Mon, 24 Oct 2022 21:57:31 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Mon, 24 Oct 2022 21:57:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Oct 2022 21:57:31 GMT
CMD ["couchbase-server"]
# Mon, 24 Oct 2022 21:57:31 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 24 Oct 2022 21:57:31 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd4213541647e0bd157630575f1ce12ab34bf86ddb1f38275d007ddee3c42e3`  
		Last Modified: Mon, 24 Oct 2022 21:58:32 GMT  
		Size: 6.1 MB (6058434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bf2e4f8352f457f4e17cefdb0a853638baf4f56e1918c045ddec2b1665ab2f`  
		Last Modified: Mon, 24 Oct 2022 21:58:31 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2b3271e89db387353725884822dba008cc472d29ce0fec112cfd2078a7100c`  
		Last Modified: Mon, 24 Oct 2022 21:59:11 GMT  
		Size: 540.8 MB (540827599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08a5945a886b16aedbd5dd6ae9b23996713053bf098818f205afea19881dbec`  
		Last Modified: Mon, 24 Oct 2022 21:58:31 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950b15f3a20c220dbcd3618f3772fd0bbdf7de89c7c3fb50627640a67bd1dff5`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 740.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727cf7782ced5c81cc91ffb1f9fb51766c5c2020061c14c87b2d3d8a12bf5c8d`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35449a251c18f484ccc31aedcb342ed8debd2e68abad0df55fed778de335c5fa`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36decd7e85da0aaf07f59bb9bc5f5dbe4d8924e028ba94e924b9199496c1b2cd`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c55cf5bd60c9cb4080ffb3224f22f72f7acf4bffefb903590a1f7b3e41977c`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:latest`

```console
$ docker pull couchbase@sha256:fb14ff77878dcc2f53b40764d8b7413268026a3a52d04ed3a06fede454e64d8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `couchbase:latest` - linux; amd64

```console
$ docker pull couchbase@sha256:43db9f11908feafb47719a0e926bfb3875efa4eb34bf233856b7e3a75778c2e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **600.1 MB (600052223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94a4e33350b160e36ed40a8ffe8424cfb308dad94279fa3e50445693d7666352`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 04 Oct 2022 23:35:12 GMT
ADD file:8faed18d471598732aa3816c8f70e227f16f4de5db6c5c32812a09141048f56d in / 
# Tue, 04 Oct 2022 23:35:12 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 16:43:58 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 05 Oct 2022 16:43:58 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 05 Oct 2022 16:43:58 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 05 Oct 2022 16:44:32 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Mon, 24 Oct 2022 21:25:59 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2
# Mon, 24 Oct 2022 21:25:59 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb
# Mon, 24 Oct 2022 21:25:59 GMT
ARG CB_SKIP_CHECKSUM=false
# Mon, 24 Oct 2022 21:25:59 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 24 Oct 2022 21:26:00 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 24 Oct 2022 21:27:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=1c7c757cf8aee87b98c96ffea1c26f4c98b6e0c053d966c8e760224030d98477            ;;          'amd64')            CB_SHA256=26fd9ae8585e0ea6637d4f1b492ed637dcf06d664a49d369e1faf0782327b3ec            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:27:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 24 Oct 2022 21:27:22 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Mon, 24 Oct 2022 21:27:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 24 Oct 2022 21:27:23 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 24 Oct 2022 21:27:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 24 Oct 2022 21:27:24 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Mon, 24 Oct 2022 21:27:24 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Mon, 24 Oct 2022 21:27:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Oct 2022 21:27:25 GMT
CMD ["couchbase-server"]
# Mon, 24 Oct 2022 21:27:25 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 24 Oct 2022 21:27:25 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:fb0b3276a519f5e7085f51c75989b287b234b3508e1524cf2cdcbc397c06ec3d`  
		Last Modified: Thu, 22 Sep 2022 20:37:52 GMT  
		Size: 28.6 MB (28574451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f6521e7788616a3d54de1df237a477200baa4fcdcbc80f1ca20102c8dac9a2`  
		Last Modified: Wed, 05 Oct 2022 16:52:36 GMT  
		Size: 6.2 MB (6232202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed4294155157022063832d043e5870cf3f0041b257eb6d0591a71ccb884e1ad`  
		Last Modified: Mon, 24 Oct 2022 21:29:40 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b75350ea80943a6d0b728ac523d24812c072e9df29e1b3dc9245795be253cdd`  
		Last Modified: Mon, 24 Oct 2022 21:30:37 GMT  
		Size: 565.2 MB (565241194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b83fd8b65df9e1924726130bc71fd564d349c9362c18c537a875332b7868199e`  
		Last Modified: Mon, 24 Oct 2022 21:29:40 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a99cbee36c8d0b15280d3e06198929d60faa79e9b8c68d8eeb0a3876496659e`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 744.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa185d8f3874bc3626d0f50eb0c3a5807922e71c9df2f2c80dcb396fd02f6d4`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 281.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1041a169a865e16423286b77033d7444428e6accaf344bbaa08ee980294ddb4d`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d34e150d092d28dd1b92731f930fe34902f1007e6d3b5281bffdd8f401de39`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53731c36206040583c501d6cafb21deff20d807630c1eec787c7506843899a6f`  
		Last Modified: Mon, 24 Oct 2022 21:29:38 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `couchbase:latest` - linux; arm64 variant v8

```console
$ docker pull couchbase@sha256:fbdbeb909ed702aa4b1ae01e65338a169fa05e2c4c9ea2f8ee68707981de72ff
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.1 MB (574082024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5586e67f79257d6baa7d552a99933db1b205b6e626eb90e54a9b2458464284e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 05 Oct 2022 00:02:10 GMT
ADD file:30b589901d2a6b82d0b7271487bdaf37514649a798cc13a17f74394321bdd051 in / 
# Wed, 05 Oct 2022 00:02:11 GMT
CMD ["bash"]
# Mon, 24 Oct 2022 21:55:44 GMT
LABEL maintainer=docker@couchbase.com
# Mon, 24 Oct 2022 21:55:44 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Mon, 24 Oct 2022 21:55:44 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:56:22 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Mon, 24 Oct 2022 21:56:22 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2
# Mon, 24 Oct 2022 21:56:23 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb
# Mon, 24 Oct 2022 21:56:23 GMT
ARG CB_SKIP_CHECKSUM=false
# Mon, 24 Oct 2022 21:56:23 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Mon, 24 Oct 2022 21:56:23 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Mon, 24 Oct 2022 21:57:20 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=1c7c757cf8aee87b98c96ffea1c26f4c98b6e0c053d966c8e760224030d98477            ;;          'amd64')            CB_SHA256=26fd9ae8585e0ea6637d4f1b492ed637dcf06d664a49d369e1faf0782327b3ec            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Mon, 24 Oct 2022 21:57:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Mon, 24 Oct 2022 21:57:29 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Mon, 24 Oct 2022 21:57:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Mon, 24 Oct 2022 21:57:30 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Mon, 24 Oct 2022 21:57:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Mon, 24 Oct 2022 21:57:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Mon, 24 Oct 2022 21:57:31 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Mon, 24 Oct 2022 21:57:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 24 Oct 2022 21:57:31 GMT
CMD ["couchbase-server"]
# Mon, 24 Oct 2022 21:57:31 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Mon, 24 Oct 2022 21:57:31 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:514fa78e57ce0d9437bc984cc36ab780c24b69da2b922bfff16737072e3e7de2`  
		Last Modified: Wed, 05 Oct 2022 00:03:51 GMT  
		Size: 27.2 MB (27191622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fd4213541647e0bd157630575f1ce12ab34bf86ddb1f38275d007ddee3c42e3`  
		Last Modified: Mon, 24 Oct 2022 21:58:32 GMT  
		Size: 6.1 MB (6058434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57bf2e4f8352f457f4e17cefdb0a853638baf4f56e1918c045ddec2b1665ab2f`  
		Last Modified: Mon, 24 Oct 2022 21:58:31 GMT  
		Size: 1.8 KB (1840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2b3271e89db387353725884822dba008cc472d29ce0fec112cfd2078a7100c`  
		Last Modified: Mon, 24 Oct 2022 21:59:11 GMT  
		Size: 540.8 MB (540827599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e08a5945a886b16aedbd5dd6ae9b23996713053bf098818f205afea19881dbec`  
		Last Modified: Mon, 24 Oct 2022 21:58:31 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:950b15f3a20c220dbcd3618f3772fd0bbdf7de89c7c3fb50627640a67bd1dff5`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 740.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727cf7782ced5c81cc91ffb1f9fb51766c5c2020061c14c87b2d3d8a12bf5c8d`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 276.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35449a251c18f484ccc31aedcb342ed8debd2e68abad0df55fed778de335c5fa`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36decd7e85da0aaf07f59bb9bc5f5dbe4d8924e028ba94e924b9199496c1b2cd`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c55cf5bd60c9cb4080ffb3224f22f72f7acf4bffefb903590a1f7b3e41977c`  
		Last Modified: Mon, 24 Oct 2022 21:58:29 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
