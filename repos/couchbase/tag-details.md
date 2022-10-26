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
$ docker pull couchbase@sha256:063e53bbcaf5ebf0dc5556ab8687960c5699099a5bfebf077a6085f0e465d058
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
$ docker pull couchbase@sha256:9a4888c0ce9651cb27020be56956c4fd3fe39cd7160fdfd8b70ca2566d34f73d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.1 MB (574088800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf41ad4fdd68f8d6b24fcded6b8c122c9dad0c51bb24da871bc1d1e539178035`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 01:03:34 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 26 Oct 2022 01:03:34 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 26 Oct 2022 01:03:34 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 26 Oct 2022 01:04:06 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 26 Oct 2022 01:04:06 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2
# Wed, 26 Oct 2022 01:04:06 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb
# Wed, 26 Oct 2022 01:04:06 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 26 Oct 2022 01:04:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 26 Oct 2022 01:04:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 26 Oct 2022 01:04:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=1c7c757cf8aee87b98c96ffea1c26f4c98b6e0c053d966c8e760224030d98477            ;;          'amd64')            CB_SHA256=26fd9ae8585e0ea6637d4f1b492ed637dcf06d664a49d369e1faf0782327b3ec            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 26 Oct 2022 01:04:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 26 Oct 2022 01:04:57 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 26 Oct 2022 01:04:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 26 Oct 2022 01:04:58 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 26 Oct 2022 01:04:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 26 Oct 2022 01:04:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 26 Oct 2022 01:04:59 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 26 Oct 2022 01:04:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Oct 2022 01:04:59 GMT
CMD ["couchbase-server"]
# Wed, 26 Oct 2022 01:04:59 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 26 Oct 2022 01:04:59 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69873e33ecff1a1e0610419e7f10325c069fab1df9314e8aac62d17307806a3`  
		Last Modified: Wed, 26 Oct 2022 01:06:05 GMT  
		Size: 6.1 MB (6059698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42689a7d037c118c8f80945e03eb3fd86160497a905592fa09c4ad52760b2b37`  
		Last Modified: Wed, 26 Oct 2022 01:06:04 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea073f8f3543b1e17d23d96c5ddee5e7e0fa40de1d6e740361a8db5b0684d9a9`  
		Last Modified: Wed, 26 Oct 2022 01:06:44 GMT  
		Size: 540.8 MB (540828733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449cffd4bc6ce1b1fa337cfb7fd331588a756d55d794a7fb1889959450bddd77`  
		Last Modified: Wed, 26 Oct 2022 01:06:04 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef5720f1eac34c77d45c499a897539d9df7a9cff9361429069c9fab9124685f`  
		Last Modified: Wed, 26 Oct 2022 01:06:02 GMT  
		Size: 743.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e51ea8f00f9893468229bde542313cf22eb5fa1412a6339966d9ed593d8431`  
		Last Modified: Wed, 26 Oct 2022 01:06:02 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcca3cf917e817b273da193851219e829d9f191e5ea52aa12cbf6747d214cb4`  
		Last Modified: Wed, 26 Oct 2022 01:06:02 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6780a517c5f36d3b34dcd2960ba09ade2a87ef09b5da610cd9f50c1124df15`  
		Last Modified: Wed, 26 Oct 2022 01:06:02 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b05bbb83aa2d245e2d34a933fdd2eeef43dbb905a169074d507b4b11dadc5d`  
		Last Modified: Wed, 26 Oct 2022 01:06:02 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community`

```console
$ docker pull couchbase@sha256:a3fe33e22870cba688c356b68f7a3b9b8cd123f60c599a297b604a15583095ce
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
$ docker pull couchbase@sha256:2f33a48159264361e561cd91383fa5caf9571e38c748204a101ee3d5fb4d23ee
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.3 MB (327287005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2873d3986a53dacc76add471a133090d2ba282b976f59209079cbb4b98221dad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 01:03:34 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 26 Oct 2022 01:03:34 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 26 Oct 2022 01:03:34 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 26 Oct 2022 01:04:06 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 26 Oct 2022 01:05:11 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1
# Wed, 26 Oct 2022 01:05:11 GMT
ARG CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb
# Wed, 26 Oct 2022 01:05:11 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 26 Oct 2022 01:05:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 26 Oct 2022 01:05:12 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 26 Oct 2022 01:05:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=275a0bb41d81920e9948fc05f736eef753179f698a04609eb8fe617d0fe55b8b            ;;          'amd64')            CB_SHA256=2fa47dc00f6d85aad5298149bb52450cc98c2c1e18eb54ab8ed45346c24a9403            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 26 Oct 2022 01:05:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 26 Oct 2022 01:05:44 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 26 Oct 2022 01:05:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 26 Oct 2022 01:05:44 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 26 Oct 2022 01:05:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 26 Oct 2022 01:05:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 26 Oct 2022 01:05:45 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 26 Oct 2022 01:05:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Oct 2022 01:05:45 GMT
CMD ["couchbase-server"]
# Wed, 26 Oct 2022 01:05:45 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 26 Oct 2022 01:05:46 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69873e33ecff1a1e0610419e7f10325c069fab1df9314e8aac62d17307806a3`  
		Last Modified: Wed, 26 Oct 2022 01:06:05 GMT  
		Size: 6.1 MB (6059698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85885eb367904d1df9d95279b28fdc48aec37f0d76f3f502f6f18d13ca174e82`  
		Last Modified: Wed, 26 Oct 2022 01:07:03 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8cf8dda76465be8b898111b87b06ed3de8116ffe7c62b1ba3c6508cfc51f19`  
		Last Modified: Wed, 26 Oct 2022 01:07:29 GMT  
		Size: 294.0 MB (294026940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46dfd409edf748867674a21db8d085c320e67e76c5cc2c5e33f20719aa89ad6`  
		Last Modified: Wed, 26 Oct 2022 01:07:02 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb370a5bd6d9b95bf80be88ad3744c9228fea4baaed1b7a274b9481f1b3c6c2`  
		Last Modified: Wed, 26 Oct 2022 01:07:01 GMT  
		Size: 742.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cef3105bb0575f2569480d8c156d9439f6a7f3e67344b944a79e54774c8b404`  
		Last Modified: Wed, 26 Oct 2022 01:07:00 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b883b2cdb33b3f0c43ac915354bd61694ca28eb3fd54660b47bdd5df7de93cba`  
		Last Modified: Wed, 26 Oct 2022 01:07:00 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c0c929056280d69ef668cb6fc451cc69cd8cc271060b97df65265405bcb5c1`  
		Last Modified: Wed, 26 Oct 2022 01:07:00 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dda6eeaa273d177fa841fb2ef279528f0cdb7dacda379ee7b81f64f41b9d14`  
		Last Modified: Wed, 26 Oct 2022 01:07:00 GMT  
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
$ docker pull couchbase@sha256:a3fe33e22870cba688c356b68f7a3b9b8cd123f60c599a297b604a15583095ce
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
$ docker pull couchbase@sha256:2f33a48159264361e561cd91383fa5caf9571e38c748204a101ee3d5fb4d23ee
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.3 MB (327287005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2873d3986a53dacc76add471a133090d2ba282b976f59209079cbb4b98221dad`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 01:03:34 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 26 Oct 2022 01:03:34 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 26 Oct 2022 01:03:34 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 26 Oct 2022 01:04:06 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 26 Oct 2022 01:05:11 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1
# Wed, 26 Oct 2022 01:05:11 GMT
ARG CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb
# Wed, 26 Oct 2022 01:05:11 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 26 Oct 2022 01:05:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 26 Oct 2022 01:05:12 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 26 Oct 2022 01:05:38 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=275a0bb41d81920e9948fc05f736eef753179f698a04609eb8fe617d0fe55b8b            ;;          'amd64')            CB_SHA256=2fa47dc00f6d85aad5298149bb52450cc98c2c1e18eb54ab8ed45346c24a9403            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 26 Oct 2022 01:05:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 26 Oct 2022 01:05:44 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 26 Oct 2022 01:05:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 26 Oct 2022 01:05:44 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 26 Oct 2022 01:05:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 26 Oct 2022 01:05:45 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.1.1-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.1 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 26 Oct 2022 01:05:45 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 26 Oct 2022 01:05:45 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Oct 2022 01:05:45 GMT
CMD ["couchbase-server"]
# Wed, 26 Oct 2022 01:05:45 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 26 Oct 2022 01:05:46 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69873e33ecff1a1e0610419e7f10325c069fab1df9314e8aac62d17307806a3`  
		Last Modified: Wed, 26 Oct 2022 01:06:05 GMT  
		Size: 6.1 MB (6059698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85885eb367904d1df9d95279b28fdc48aec37f0d76f3f502f6f18d13ca174e82`  
		Last Modified: Wed, 26 Oct 2022 01:07:03 GMT  
		Size: 1.8 KB (1841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a8cf8dda76465be8b898111b87b06ed3de8116ffe7c62b1ba3c6508cfc51f19`  
		Last Modified: Wed, 26 Oct 2022 01:07:29 GMT  
		Size: 294.0 MB (294026940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46dfd409edf748867674a21db8d085c320e67e76c5cc2c5e33f20719aa89ad6`  
		Last Modified: Wed, 26 Oct 2022 01:07:02 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eb370a5bd6d9b95bf80be88ad3744c9228fea4baaed1b7a274b9481f1b3c6c2`  
		Last Modified: Wed, 26 Oct 2022 01:07:01 GMT  
		Size: 742.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cef3105bb0575f2569480d8c156d9439f6a7f3e67344b944a79e54774c8b404`  
		Last Modified: Wed, 26 Oct 2022 01:07:00 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b883b2cdb33b3f0c43ac915354bd61694ca28eb3fd54660b47bdd5df7de93cba`  
		Last Modified: Wed, 26 Oct 2022 01:07:00 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c0c929056280d69ef668cb6fc451cc69cd8cc271060b97df65265405bcb5c1`  
		Last Modified: Wed, 26 Oct 2022 01:07:00 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05dda6eeaa273d177fa841fb2ef279528f0cdb7dacda379ee7b81f64f41b9d14`  
		Last Modified: Wed, 26 Oct 2022 01:07:00 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise`

```console
$ docker pull couchbase@sha256:063e53bbcaf5ebf0dc5556ab8687960c5699099a5bfebf077a6085f0e465d058
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
$ docker pull couchbase@sha256:9a4888c0ce9651cb27020be56956c4fd3fe39cd7160fdfd8b70ca2566d34f73d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.1 MB (574088800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf41ad4fdd68f8d6b24fcded6b8c122c9dad0c51bb24da871bc1d1e539178035`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 01:03:34 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 26 Oct 2022 01:03:34 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 26 Oct 2022 01:03:34 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 26 Oct 2022 01:04:06 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 26 Oct 2022 01:04:06 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2
# Wed, 26 Oct 2022 01:04:06 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb
# Wed, 26 Oct 2022 01:04:06 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 26 Oct 2022 01:04:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 26 Oct 2022 01:04:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 26 Oct 2022 01:04:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=1c7c757cf8aee87b98c96ffea1c26f4c98b6e0c053d966c8e760224030d98477            ;;          'amd64')            CB_SHA256=26fd9ae8585e0ea6637d4f1b492ed637dcf06d664a49d369e1faf0782327b3ec            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 26 Oct 2022 01:04:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 26 Oct 2022 01:04:57 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 26 Oct 2022 01:04:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 26 Oct 2022 01:04:58 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 26 Oct 2022 01:04:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 26 Oct 2022 01:04:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 26 Oct 2022 01:04:59 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 26 Oct 2022 01:04:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Oct 2022 01:04:59 GMT
CMD ["couchbase-server"]
# Wed, 26 Oct 2022 01:04:59 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 26 Oct 2022 01:04:59 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69873e33ecff1a1e0610419e7f10325c069fab1df9314e8aac62d17307806a3`  
		Last Modified: Wed, 26 Oct 2022 01:06:05 GMT  
		Size: 6.1 MB (6059698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42689a7d037c118c8f80945e03eb3fd86160497a905592fa09c4ad52760b2b37`  
		Last Modified: Wed, 26 Oct 2022 01:06:04 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea073f8f3543b1e17d23d96c5ddee5e7e0fa40de1d6e740361a8db5b0684d9a9`  
		Last Modified: Wed, 26 Oct 2022 01:06:44 GMT  
		Size: 540.8 MB (540828733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449cffd4bc6ce1b1fa337cfb7fd331588a756d55d794a7fb1889959450bddd77`  
		Last Modified: Wed, 26 Oct 2022 01:06:04 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef5720f1eac34c77d45c499a897539d9df7a9cff9361429069c9fab9124685f`  
		Last Modified: Wed, 26 Oct 2022 01:06:02 GMT  
		Size: 743.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e51ea8f00f9893468229bde542313cf22eb5fa1412a6339966d9ed593d8431`  
		Last Modified: Wed, 26 Oct 2022 01:06:02 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcca3cf917e817b273da193851219e829d9f191e5ea52aa12cbf6747d214cb4`  
		Last Modified: Wed, 26 Oct 2022 01:06:02 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6780a517c5f36d3b34dcd2960ba09ade2a87ef09b5da610cd9f50c1124df15`  
		Last Modified: Wed, 26 Oct 2022 01:06:02 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b05bbb83aa2d245e2d34a933fdd2eeef43dbb905a169074d507b4b11dadc5d`  
		Last Modified: Wed, 26 Oct 2022 01:06:02 GMT  
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
$ docker pull couchbase@sha256:063e53bbcaf5ebf0dc5556ab8687960c5699099a5bfebf077a6085f0e465d058
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
$ docker pull couchbase@sha256:9a4888c0ce9651cb27020be56956c4fd3fe39cd7160fdfd8b70ca2566d34f73d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.1 MB (574088800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf41ad4fdd68f8d6b24fcded6b8c122c9dad0c51bb24da871bc1d1e539178035`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 01:03:34 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 26 Oct 2022 01:03:34 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 26 Oct 2022 01:03:34 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 26 Oct 2022 01:04:06 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 26 Oct 2022 01:04:06 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2
# Wed, 26 Oct 2022 01:04:06 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb
# Wed, 26 Oct 2022 01:04:06 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 26 Oct 2022 01:04:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 26 Oct 2022 01:04:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 26 Oct 2022 01:04:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=1c7c757cf8aee87b98c96ffea1c26f4c98b6e0c053d966c8e760224030d98477            ;;          'amd64')            CB_SHA256=26fd9ae8585e0ea6637d4f1b492ed637dcf06d664a49d369e1faf0782327b3ec            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 26 Oct 2022 01:04:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 26 Oct 2022 01:04:57 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 26 Oct 2022 01:04:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 26 Oct 2022 01:04:58 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 26 Oct 2022 01:04:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 26 Oct 2022 01:04:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 26 Oct 2022 01:04:59 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 26 Oct 2022 01:04:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Oct 2022 01:04:59 GMT
CMD ["couchbase-server"]
# Wed, 26 Oct 2022 01:04:59 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 26 Oct 2022 01:04:59 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69873e33ecff1a1e0610419e7f10325c069fab1df9314e8aac62d17307806a3`  
		Last Modified: Wed, 26 Oct 2022 01:06:05 GMT  
		Size: 6.1 MB (6059698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42689a7d037c118c8f80945e03eb3fd86160497a905592fa09c4ad52760b2b37`  
		Last Modified: Wed, 26 Oct 2022 01:06:04 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea073f8f3543b1e17d23d96c5ddee5e7e0fa40de1d6e740361a8db5b0684d9a9`  
		Last Modified: Wed, 26 Oct 2022 01:06:44 GMT  
		Size: 540.8 MB (540828733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449cffd4bc6ce1b1fa337cfb7fd331588a756d55d794a7fb1889959450bddd77`  
		Last Modified: Wed, 26 Oct 2022 01:06:04 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef5720f1eac34c77d45c499a897539d9df7a9cff9361429069c9fab9124685f`  
		Last Modified: Wed, 26 Oct 2022 01:06:02 GMT  
		Size: 743.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e51ea8f00f9893468229bde542313cf22eb5fa1412a6339966d9ed593d8431`  
		Last Modified: Wed, 26 Oct 2022 01:06:02 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcca3cf917e817b273da193851219e829d9f191e5ea52aa12cbf6747d214cb4`  
		Last Modified: Wed, 26 Oct 2022 01:06:02 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6780a517c5f36d3b34dcd2960ba09ade2a87ef09b5da610cd9f50c1124df15`  
		Last Modified: Wed, 26 Oct 2022 01:06:02 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b05bbb83aa2d245e2d34a933fdd2eeef43dbb905a169074d507b4b11dadc5d`  
		Last Modified: Wed, 26 Oct 2022 01:06:02 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:latest`

```console
$ docker pull couchbase@sha256:063e53bbcaf5ebf0dc5556ab8687960c5699099a5bfebf077a6085f0e465d058
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
$ docker pull couchbase@sha256:9a4888c0ce9651cb27020be56956c4fd3fe39cd7160fdfd8b70ca2566d34f73d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **574.1 MB (574088800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf41ad4fdd68f8d6b24fcded6b8c122c9dad0c51bb24da871bc1d1e539178035`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Tue, 25 Oct 2022 05:54:59 GMT
ADD file:6784d0c4432f4f32d6ee4d96eedf33ea82d88ef6901c763665fa77c842621999 in / 
# Tue, 25 Oct 2022 05:54:59 GMT
CMD ["bash"]
# Wed, 26 Oct 2022 01:03:34 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 26 Oct 2022 01:03:34 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 26 Oct 2022 01:03:34 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 26 Oct 2022 01:04:06 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 26 Oct 2022 01:04:06 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2
# Wed, 26 Oct 2022 01:04:06 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb
# Wed, 26 Oct 2022 01:04:06 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 26 Oct 2022 01:04:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 26 Oct 2022 01:04:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 26 Oct 2022 01:04:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && dpkgArch="$(dpkg --print-architecture)"     && case "${dpkgArch}" in          'arm64')            CB_SHA256=1c7c757cf8aee87b98c96ffea1c26f4c98b6e0c053d966c8e760224030d98477            ;;          'amd64')            CB_SHA256=26fd9ae8585e0ea6637d4f1b492ed637dcf06d664a49d369e1faf0782327b3ec            ;;        esac     && CB_PACKAGE=$(echo ${CB_PACKAGE} | sed -e "s/@@ARCH@@/${dpkgArch}/")     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 26 Oct 2022 01:04:57 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 26 Oct 2022 01:04:57 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 26 Oct 2022 01:04:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 26 Oct 2022 01:04:58 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 26 Oct 2022 01:04:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 26 Oct 2022 01:04:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.1.2-linux_@@ARCH@@.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.1.2 CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 26 Oct 2022 01:04:59 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 26 Oct 2022 01:04:59 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 26 Oct 2022 01:04:59 GMT
CMD ["couchbase-server"]
# Wed, 26 Oct 2022 01:04:59 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 26 Oct 2022 01:04:59 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:4e7e0215f4adc2c48ad9cb3b3781e21d474b477587f85682c2e2975ae91dce9d`  
		Last Modified: Tue, 25 Oct 2022 05:55:59 GMT  
		Size: 27.2 MB (27195998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b69873e33ecff1a1e0610419e7f10325c069fab1df9314e8aac62d17307806a3`  
		Last Modified: Wed, 26 Oct 2022 01:06:05 GMT  
		Size: 6.1 MB (6059698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42689a7d037c118c8f80945e03eb3fd86160497a905592fa09c4ad52760b2b37`  
		Last Modified: Wed, 26 Oct 2022 01:06:04 GMT  
		Size: 1.8 KB (1839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea073f8f3543b1e17d23d96c5ddee5e7e0fa40de1d6e740361a8db5b0684d9a9`  
		Last Modified: Wed, 26 Oct 2022 01:06:44 GMT  
		Size: 540.8 MB (540828733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449cffd4bc6ce1b1fa337cfb7fd331588a756d55d794a7fb1889959450bddd77`  
		Last Modified: Wed, 26 Oct 2022 01:06:04 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef5720f1eac34c77d45c499a897539d9df7a9cff9361429069c9fab9124685f`  
		Last Modified: Wed, 26 Oct 2022 01:06:02 GMT  
		Size: 743.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e51ea8f00f9893468229bde542313cf22eb5fa1412a6339966d9ed593d8431`  
		Last Modified: Wed, 26 Oct 2022 01:06:02 GMT  
		Size: 280.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fcca3cf917e817b273da193851219e829d9f191e5ea52aa12cbf6747d214cb4`  
		Last Modified: Wed, 26 Oct 2022 01:06:02 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f6780a517c5f36d3b34dcd2960ba09ade2a87ef09b5da610cd9f50c1124df15`  
		Last Modified: Wed, 26 Oct 2022 01:06:02 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b05bbb83aa2d245e2d34a933fdd2eeef43dbb905a169074d507b4b11dadc5d`  
		Last Modified: Wed, 26 Oct 2022 01:06:02 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
