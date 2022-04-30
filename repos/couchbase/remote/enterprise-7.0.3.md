## `couchbase:enterprise-7.0.3`

```console
$ docker pull couchbase@sha256:09d0fb59d4f8df68a5a5352bbb172cb41608eb961e1ede38c41b044cb2359461
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-7.0.3` - linux; amd64

```console
$ docker pull couchbase@sha256:cc0a5a62c8664ba8684335f195650691b6476a99be5849805d5a13ba572ab9e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **653.6 MB (653562427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24f8a22a0df0012dc1a1270128f1a15a4ee18a95e7f7f253b413dd92181cc97a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 29 Apr 2022 23:20:59 GMT
ADD file:7009ad0ee0bbe5ed7f381792e07347e260e6896aeee0d80597808065120fa96b in / 
# Fri, 29 Apr 2022 23:20:59 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:04:47 GMT
LABEL maintainer=docker@couchbase.com
# Sat, 30 Apr 2022 00:04:47 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Sat, 30 Apr 2022 00:04:48 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:05:04 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Sat, 30 Apr 2022 00:05:04 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1
# Sat, 30 Apr 2022 00:05:04 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb
# Sat, 30 Apr 2022 00:05:04 GMT
ARG CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f
# Sat, 30 Apr 2022 00:05:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Sat, 30 Apr 2022 00:05:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Sat, 30 Apr 2022 00:07:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c -     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Sat, 30 Apr 2022 00:07:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Sat, 30 Apr 2022 00:07:07 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Sat, 30 Apr 2022 00:07:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Sat, 30 Apr 2022 00:07:07 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Sat, 30 Apr 2022 00:07:08 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Sat, 30 Apr 2022 00:07:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.3-MP1-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.3-MP1 CB_SHA256=a1bfcc476e01c71a212c2ed5026f24f3df01b3591c24dcf45678fdb2625cfc0f CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Sat, 30 Apr 2022 00:07:14 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Sat, 30 Apr 2022 00:07:14 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 30 Apr 2022 00:07:15 GMT
CMD ["couchbase-server"]
# Sat, 30 Apr 2022 00:07:15 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Sat, 30 Apr 2022 00:07:15 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:d5fd17ec1767521cf97f61568096bfc9a7cd9c2d149576a7b43930c5a97062b0`  
		Last Modified: Thu, 28 Apr 2022 03:03:21 GMT  
		Size: 28.6 MB (28566230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76937b0923f63ef62ef0ce2435f73244f7f909cc74136aba1228f2e2574af748`  
		Last Modified: Sat, 30 Apr 2022 00:18:06 GMT  
		Size: 6.3 MB (6250617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce99684904adf2c3f56e5d7abd675e5cf6a024381ea64a827e805e2022974da6`  
		Last Modified: Sat, 30 Apr 2022 00:18:05 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff533d3886c8143e80c8fcce9834656e1796453ca5f6e579442e59e644fb9aa8`  
		Last Modified: Sat, 30 Apr 2022 00:19:09 GMT  
		Size: 618.3 MB (618297660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244f8c789e91a9b9c853463ba29dfb9da147c72b8d9bf54e5e3b0b34ae85d84a`  
		Last Modified: Sat, 30 Apr 2022 00:18:05 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ac7ffc32bcefda82cafad3d09e24ff3bb1643231bf1c5df473999927f9a0029`  
		Last Modified: Sat, 30 Apr 2022 00:18:05 GMT  
		Size: 736.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fbe28691c5e53c547e3f6750a7300ccb0f093986c50167e69281f51db18b2b2`  
		Last Modified: Sat, 30 Apr 2022 00:18:02 GMT  
		Size: 277.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b46d9ecfa389b345724069f06b58b43916e7ad0d55d6b757729079a2e77337`  
		Last Modified: Sat, 30 Apr 2022 00:18:02 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a747a0b4e81b2d4a1436f1498f57d42f9ae15b9d4126e6d9ced78261052955c1`  
		Last Modified: Sat, 30 Apr 2022 00:18:03 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e71663811e7ab33e06489f5a666fcc8174db799b918054c69565853d630a8f2`  
		Last Modified: Sat, 30 Apr 2022 00:18:03 GMT  
		Size: 443.6 KB (443560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f20164e41e2fec4dc4897c33ac3ad902b50c2d83da7c0e19a4f85c566323b12`  
		Last Modified: Sat, 30 Apr 2022 00:18:02 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
