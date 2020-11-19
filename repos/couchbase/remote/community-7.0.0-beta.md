## `couchbase:community-7.0.0-beta`

```console
$ docker pull couchbase@sha256:92e33bc0f25b378ac83dbd457e5e7c0872dd19cdcc8ee6aa756a4618336954cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:community-7.0.0-beta` - linux; amd64

```console
$ docker pull couchbase@sha256:6a3a0f89bf1cb2d9a423e4bdf89b0b873d0ba37cb9a366192e05941bb8dc9d2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.4 MB (427391262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44fbd26be83497318843a6387ab73f3bf3559e930089b380c70389ee770dbe9d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 23 Oct 2020 17:32:33 GMT
ADD file:435d9776fdd3a1834f344fb82e459dbbb67cd50c71ab5e29b719273888d5bb7c in / 
# Fri, 23 Oct 2020 17:32:34 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:32:35 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 23 Oct 2020 17:32:36 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:32:36 GMT
CMD ["/bin/bash"]
# Wed, 18 Nov 2020 16:57:23 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Wed, 18 Nov 2020 16:57:45 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 18 Nov 2020 16:57:46 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 18 Nov 2020 16:57:46 GMT
ARG CB_VERSION=7.0.0-beta
# Wed, 18 Nov 2020 16:57:46 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta
# Wed, 18 Nov 2020 16:59:24 GMT
ARG CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb
# Wed, 18 Nov 2020 16:59:24 GMT
ARG CB_SHA256=7b2c5ec52ee2dd3d9e3af6943324cc0dfede0455bbc4e9c3839f4f76786ab900
# Wed, 18 Nov 2020 16:59:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 18 Nov 2020 16:59:25 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=7b2c5ec52ee2dd3d9e3af6943324cc0dfede0455bbc4e9c3839f4f76786ab900 CB_VERSION=7.0.0-beta
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 18 Nov 2020 17:00:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=7b2c5ec52ee2dd3d9e3af6943324cc0dfede0455bbc4e9c3839f4f76786ab900 CB_VERSION=7.0.0-beta
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Wed, 18 Nov 2020 17:00:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=7b2c5ec52ee2dd3d9e3af6943324cc0dfede0455bbc4e9c3839f4f76786ab900 CB_VERSION=7.0.0-beta
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 18 Nov 2020 17:00:17 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 18 Nov 2020 17:00:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=7b2c5ec52ee2dd3d9e3af6943324cc0dfede0455bbc4e9c3839f4f76786ab900 CB_VERSION=7.0.0-beta
RUN chown -R couchbase:couchbase /etc/service
# Wed, 18 Nov 2020 17:00:18 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 18 Nov 2020 17:00:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=7b2c5ec52ee2dd3d9e3af6943324cc0dfede0455bbc4e9c3839f4f76786ab900 CB_VERSION=7.0.0-beta
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 18 Nov 2020 17:00:20 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=7b2c5ec52ee2dd3d9e3af6943324cc0dfede0455bbc4e9c3839f4f76786ab900 CB_VERSION=7.0.0-beta
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 18 Nov 2020 17:00:20 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 18 Nov 2020 17:00:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Nov 2020 17:00:21 GMT
CMD ["couchbase-server"]
# Wed, 18 Nov 2020 17:00:21 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 18 Nov 2020 17:00:21 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:6a5697faee43339ef8e33e3839060252392ad99325a48f7c9d7e93c22db4d4cf`  
		Last Modified: Thu, 08 Oct 2020 15:19:51 GMT  
		Size: 28.6 MB (28558714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba13d3bc422b493440f97a8f148d245e1999cb616cb05876edc3ef29e79852f2`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a254829d9e55168306fd80a49e02eb015551facee9c444d9dce3b26d19238b82`  
		Last Modified: Fri, 23 Oct 2020 17:33:25 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd318becfee372f6b5cc45b8a51d4a977487c3debf46a312e01190149ef43b25`  
		Last Modified: Wed, 18 Nov 2020 17:00:50 GMT  
		Size: 6.3 MB (6277441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22791c930af70b06b0d0c54ace5bce00374d540a311e0d6b3915a2d78feffd42`  
		Last Modified: Wed, 18 Nov 2020 17:00:46 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74215dfca2fac6d0f7331510afcddf993eb6ae63e8c8ed047aec90f3601de770`  
		Last Modified: Wed, 18 Nov 2020 17:02:12 GMT  
		Size: 1.8 KB (1837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4884ac72241b82e2530a0f85d37bcaa465269c98391b67f1fc261ab4ecaf8a86`  
		Last Modified: Wed, 18 Nov 2020 17:03:10 GMT  
		Size: 392.4 MB (392424000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb86f71585d5c120e1e6c8186dd08524e695622c2f0ca577029a01f69b5bbcd`  
		Last Modified: Wed, 18 Nov 2020 17:02:12 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49a30fd6b3e86d479af9f33bfe551c6c1d69de9864663e4467b3bb17cd6f800`  
		Last Modified: Wed, 18 Nov 2020 17:02:12 GMT  
		Size: 451.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708c8413ee838bcb5f29c28cb1e5b8dea81ac9c2b402cb256a41f886241b3890`  
		Last Modified: Wed, 18 Nov 2020 17:02:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac5bdd241263eaca859ec2f517cef53f77b35602136bdc440d420fb64c5a204`  
		Last Modified: Wed, 18 Nov 2020 17:02:10 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ab90d81dd1f3951842ff637f53eddec414024fccac797a60f7395c59f4fa21`  
		Last Modified: Wed, 18 Nov 2020 17:02:11 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c431114583e247c47231feb19ce2540a78e0fe2af9f0797656ab288afd7405c6`  
		Last Modified: Wed, 18 Nov 2020 17:02:11 GMT  
		Size: 125.9 KB (125890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64d44aed69eebd8686b67a48518ae2e4c353a6fda304ca5ec53253f7b3ded8a`  
		Last Modified: Wed, 18 Nov 2020 17:02:11 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
