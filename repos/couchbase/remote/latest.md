## `couchbase:latest`

```console
$ docker pull couchbase@sha256:7b3d5fab2ce0874e3c9c592fef5b23e9261761771544777d58da7dd5a5d2a8a8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:latest` - linux; amd64

```console
$ docker pull couchbase@sha256:33a751f77c73af46530e28d23b15a1610df2076ce294698792b467e1a2a1173a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **541.8 MB (541762006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0266a58ce0e676e3aab9b96f83a06875ebe3c80de6e75c84d74d605b3fa6252`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Wed, 16 Sep 2020 22:22:41 GMT
ADD file:22e6fa4e90b4c26ba962a4fe57e5784d8923885e6eb39435cb121c716c42f7ff in / 
# Wed, 16 Sep 2020 22:22:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 16 Sep 2020 22:22:43 GMT
RUN rm -rf /var/lib/apt/lists/*
# Wed, 16 Sep 2020 22:22:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 16 Sep 2020 22:22:44 GMT
CMD ["/bin/bash"]
# Wed, 16 Sep 2020 23:56:12 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Wed, 16 Sep 2020 23:56:31 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Wed, 16 Sep 2020 23:56:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Wed, 16 Sep 2020 23:56:32 GMT
ARG CB_VERSION=6.6.0
# Wed, 16 Sep 2020 23:56:32 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Wed, 16 Sep 2020 23:56:32 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb
# Wed, 16 Sep 2020 23:56:33 GMT
ARG CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9
# Wed, 16 Sep 2020 23:56:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 16 Sep 2020 23:56:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 16 Sep 2020 23:57:29 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Wed, 16 Sep 2020 23:57:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 16 Sep 2020 23:57:30 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 16 Sep 2020 23:57:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN chown -R couchbase:couchbase /etc/service
# Wed, 16 Sep 2020 23:57:31 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 16 Sep 2020 23:57:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 16 Sep 2020 23:57:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 16 Sep 2020 23:57:33 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 16 Sep 2020 23:57:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 16 Sep 2020 23:57:33 GMT
CMD ["couchbase-server"]
# Wed, 16 Sep 2020 23:57:33 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 16 Sep 2020 23:57:33 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:001ecc9468da6632359722ccefa732463486659ee07daacd31602ec3bf4d862f`  
		Last Modified: Fri, 04 Sep 2020 13:20:12 GMT  
		Size: 44.5 MB (44490811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b9667498691604756cf3601ba44360f2b1f6ba8b5745eee963847d2a4ea736`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe474042557a4bffb655cd6079656d79e2ecfb0d0fad367c610ca1ec65d0e86`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1bf2fb0fbbc55e614a3391455d772eae373e0136b7cba4d79dd72f28fb347f0`  
		Last Modified: Wed, 16 Sep 2020 22:23:34 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32eccc2ee7be53bd8bfe8fd2f20d84ad2b1a4d4890354127dcfb1ccb05e8c208`  
		Last Modified: Thu, 17 Sep 2020 00:00:20 GMT  
		Size: 5.8 MB (5827160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8749ec1c1e66c99f8c42155075d7d208921a2fbaed312f6e617d6c4680ca6309`  
		Last Modified: Thu, 17 Sep 2020 00:00:17 GMT  
		Size: 2.1 KB (2076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136c14103702b8a956b670448832897668f7443ec26b2095328977319b292f09`  
		Last Modified: Thu, 17 Sep 2020 00:01:16 GMT  
		Size: 491.3 MB (491320019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2eba528fabb0e5775adb78a07d1042681331ac5b287eb22d6c7f93626cb60cc`  
		Last Modified: Thu, 17 Sep 2020 00:00:16 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad65d688c797084d4f1e7b558eb0cb4b8fee1714c2374108b7190aacd114cb18`  
		Last Modified: Thu, 17 Sep 2020 00:00:16 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b159bd9951b4e16aae619e1928df4f2ab52ba7db335b2d476f438844375bd88f`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2c2e784af48b204685a2ab2072fe714c90517ed7ebbc515e3afb13cf593cbfb`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffc8117c5c55028c9eb93a77d7bbb49c5a8f31927384dde9383ddea26ca32e0`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8487384ac1cb40b5b5b3d0bd457fa8bee0dbcd3b83eb395f47592596cb0e5fca`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 118.1 KB (118072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e0171f2f8d3d6117b7b9f6fb9d3e98288702d75bf8fef4bfb808b443a9273a1`  
		Last Modified: Thu, 17 Sep 2020 00:00:14 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
