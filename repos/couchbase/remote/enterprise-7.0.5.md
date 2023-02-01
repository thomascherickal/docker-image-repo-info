## `couchbase:enterprise-7.0.5`

```console
$ docker pull couchbase@sha256:70d1600c289c834e69caaea2c8c981b5a9ebc245e91d6d729bd333e77f95c072
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `couchbase:enterprise-7.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:afa70468149f42aa257d2fdc35c6b4d748dfe077abd7f101a040ec5080b119d6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **616.6 MB (616628710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c670efa3cc51d5c7a1ae1bef657131d726a397c150d225219e0593613b5dc0e`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 01 Feb 2023 11:42:37 GMT
ARG RELEASE
# Wed, 01 Feb 2023 11:42:37 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 01 Feb 2023 11:42:37 GMT
LABEL org.opencontainers.image.version=20.04
# Wed, 01 Feb 2023 11:42:39 GMT
ADD file:8b180a9b4497de0c6e131d6b48cf5c69a885379e63033ab9639d1655991e626c in / 
# Wed, 01 Feb 2023 11:42:39 GMT
CMD ["/bin/bash"]
# Wed, 01 Feb 2023 18:25:04 GMT
LABEL maintainer=docker@couchbase.com
# Wed, 01 Feb 2023 18:25:04 GMT
ARG UPDATE_COMMAND=apt-get update -y -q
# Wed, 01 Feb 2023 18:25:04 GMT
ARG CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:25:27 GMT
# ARGS: CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ${UPDATE_COMMAND}     && apt-get install -y -q wget tzdata       lsof lshw sysstat net-tools numactl bzip2 runit     && ${CLEANUP_COMMAND}
# Wed, 01 Feb 2023 18:27:30 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5
# Wed, 01 Feb 2023 18:27:30 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb
# Wed, 01 Feb 2023 18:27:31 GMT
ARG CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea
# Wed, 01 Feb 2023 18:27:31 GMT
ARG CB_SKIP_CHECKSUM=false
# Wed, 01 Feb 2023 18:27:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 01 Feb 2023 18:27:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 01 Feb 2023 18:28:26 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && export INSTALL_DONT_START_SERVER=1     && wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE     && { ${CB_SKIP_CHECKSUM} || echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - ; }     && ${UPDATE_COMMAND}     && apt-get install -y ./$CB_PACKAGE     && rm -f ./$CB_PACKAGE     && ${CLEANUP_COMMAND}     && rm -rf /tmp/* /var/tmp/*
# Wed, 01 Feb 2023 18:28:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 01 Feb 2023 18:28:31 GMT
COPY file:018fa38d92aa0a4679f57c2d43b5c14547b2c603cab6ec7fd3240af5545472b5 in /etc/service/couchbase-server/run 
# Wed, 01 Feb 2023 18:28:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && mkdir -p /etc/runit/runsvdir/default/couchbase-server/supervise     && chown -R couchbase:couchbase                 /etc/service                 /etc/runit/runsvdir/default/couchbase-server/supervise
# Wed, 01 Feb 2023 18:28:31 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 01 Feb 2023 18:28:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -x     && ln -s dummy.sh /usr/local/bin/iptables-save     && ln -s dummy.sh /usr/local/bin/lvdisplay     && ln -s dummy.sh /usr/local/bin/vgdisplay     && ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 01 Feb 2023 18:28:33 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.5-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.5 CB_SHA256=9a5ea4e5ec6e9af81b39d1e04b135fd5e8ce13a64cd9c8d587fe3e906c17cdea CB_SKIP_CHECKSUM=false CLEANUP_COMMAND=rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* UPDATE_COMMAND=apt-get update -y -q
RUN set -ex     &&  if [ ! -e /opt/couchbase/bin/curl.real ]; then             ${UPDATE_COMMAND};             apt-get install -y chrpath;             chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl;             apt-get remove -y chrpath;             apt-get autoremove -y;             ${CLEANUP_COMMAND};         fi
# Wed, 01 Feb 2023 18:28:33 GMT
COPY file:6e5292e89c7124e038a0d80ea3b942bff1ed578e67a07e764b041ea95b129aa3 in / 
# Wed, 01 Feb 2023 18:28:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 01 Feb 2023 18:28:33 GMT
CMD ["couchbase-server"]
# Wed, 01 Feb 2023 18:28:33 GMT
EXPOSE 11207 11210 11280 18091 18092 18093 18094 18095 18096 18097 8091 8092 8093 8094 8095 8096 8097 9123
# Wed, 01 Feb 2023 18:28:33 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:7608715873ec5c02d370e963aa9b19a149023ce218887221d93fe671b3abbf58`  
		Last Modified: Thu, 26 Jan 2023 17:04:53 GMT  
		Size: 28.6 MB (28577884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b4cf586c4b7a57fc5e73b3aa283d12081f9bd7606b6b60d897f2783e6efa0d`  
		Last Modified: Wed, 01 Feb 2023 18:31:06 GMT  
		Size: 6.2 MB (6216449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507b7a7e538510c11f6158504c6a0cc9e16b8dd599ac2f8515b103b246de8e21`  
		Last Modified: Wed, 01 Feb 2023 18:33:05 GMT  
		Size: 1.8 KB (1834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de73b439ff8a91b36710c23edc8ca56c4e921ef41b2e6cb71224ea3b546b3aa`  
		Last Modified: Wed, 01 Feb 2023 18:34:03 GMT  
		Size: 581.8 MB (581830013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0738cfd3ccb6b0abfd4708b88a453af4c05a739ed6058036452db84dd98c54`  
		Last Modified: Wed, 01 Feb 2023 18:33:05 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81320e19b263a40ecbae84dfcba6bd77c9d19dcb14dc1b9633db54316234e955`  
		Last Modified: Wed, 01 Feb 2023 18:33:03 GMT  
		Size: 741.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a5e61bf65fb7021f8f7fd08cc267e9e3d2bab7e16ead1a46300ae4fa8bd4fe0`  
		Last Modified: Wed, 01 Feb 2023 18:33:03 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d065117ea502454506cbd8e4c642c1a45641130b86465e564daa4dade7b495a`  
		Last Modified: Wed, 01 Feb 2023 18:33:03 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06ef5abe6b3270b049506d26a9c2b97d6470bdd23f5004da355c317a9e076005`  
		Last Modified: Wed, 01 Feb 2023 18:33:03 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85caa0ee6487d6e3f055aa6ccb1420be7f7e05020ab26456a63a9fe63b655b62`  
		Last Modified: Wed, 01 Feb 2023 18:33:03 GMT  
		Size: 868.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
