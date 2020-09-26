## `couchbase:latest`

```console
$ docker pull couchbase@sha256:2a53dbc34039db21e08a795c1a78cb0bab8bd2e8ab91ee5077548e7e476c7e1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:latest` - linux; amd64

```console
$ docker pull couchbase@sha256:f2cb801da0c85ba9656b8f4d59f8b189c56599ec7d083a01b309540677815f25
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **541.8 MB (541788291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52d53315bb115e3426a5a87955b2853068b4d16a12742ed070002f8760ecc74b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 25 Sep 2020 22:36:27 GMT
ADD file:23a55d7e93b396e490b6d0893137e5c13e3e0a234e0feaea8b1cfd4079fb1882 in / 
# Fri, 25 Sep 2020 22:36:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 22:36:28 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 25 Sep 2020 22:36:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 22:36:29 GMT
CMD ["/bin/bash"]
# Fri, 25 Sep 2020 23:44:15 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Fri, 25 Sep 2020 23:44:31 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 25 Sep 2020 23:44:32 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Fri, 25 Sep 2020 23:44:32 GMT
ARG CB_VERSION=6.6.0
# Fri, 25 Sep 2020 23:44:32 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Fri, 25 Sep 2020 23:44:33 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb
# Fri, 25 Sep 2020 23:44:33 GMT
ARG CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9
# Fri, 25 Sep 2020 23:44:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 25 Sep 2020 23:44:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 25 Sep 2020 23:45:30 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Fri, 25 Sep 2020 23:45:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 25 Sep 2020 23:45:31 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 25 Sep 2020 23:45:32 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN chown -R couchbase:couchbase /etc/service
# Fri, 25 Sep 2020 23:45:32 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 25 Sep 2020 23:45:33 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 25 Sep 2020 23:45:34 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 25 Sep 2020 23:45:34 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 25 Sep 2020 23:45:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 25 Sep 2020 23:45:34 GMT
CMD ["couchbase-server"]
# Fri, 25 Sep 2020 23:45:35 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 25 Sep 2020 23:45:35 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:4f53fa4d2cf0e29c6a522433e0ac71a7ce0fdab158481052b2198b5518b83248`  
		Last Modified: Thu, 17 Sep 2020 13:19:58 GMT  
		Size: 44.5 MB (44517215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af7c939e38e8e3160fbbdcc26a32669529b962c79f7337df0a26bf0e9a76d59`  
		Last Modified: Fri, 25 Sep 2020 22:37:21 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903d0ffd64f6ca1355d2b2df702fc674f5663981dfd100fe4588fb390dd3382c`  
		Last Modified: Fri, 25 Sep 2020 22:37:21 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04feeed388b71fdca5cc3bce619d65a34f8a1a3e5b0ef03f8392d499970818eb`  
		Last Modified: Fri, 25 Sep 2020 22:37:21 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13321097455f75b3a691364c922ef008a0f31ae48e80095437db909e1ec50278`  
		Last Modified: Fri, 25 Sep 2020 23:48:05 GMT  
		Size: 5.8 MB (5827091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06e5881f2bd13d108bc9f009c442fc21a1ca1ade8ba0f82c1be8db438cdfc28`  
		Last Modified: Fri, 25 Sep 2020 23:48:03 GMT  
		Size: 2.1 KB (2074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d837fb506197735c0856a3f5be333f033bc48f85ec6a6857fcc3b79d54857546`  
		Last Modified: Fri, 25 Sep 2020 23:49:03 GMT  
		Size: 491.3 MB (491319972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745c1b6a70dc5fc242fd34eb1c41d67e657988223c913f1e4fd682ec891a2db2`  
		Last Modified: Fri, 25 Sep 2020 23:48:04 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3997256a47b413a650ec76da43d30f52ace3506eb8d759201451f12a7a4d08d`  
		Last Modified: Fri, 25 Sep 2020 23:48:04 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa222c9494358ca516ac0bf595892ec90456c87549937601981c16a3d10d5d2`  
		Last Modified: Fri, 25 Sep 2020 23:48:02 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76636f72b6f1a7671917e8e07ba3880e10d988c86d2336ee8b820266197a0b90`  
		Last Modified: Fri, 25 Sep 2020 23:48:02 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:649aa4826407ea384473c1fb228fa95235008fb84d3c14092cc81806fbf99f0f`  
		Last Modified: Fri, 25 Sep 2020 23:48:02 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0d0cc0df67ec7707c592dd2fa1a3ae988de3d02a5ab614e9f9b3e1a1398a03`  
		Last Modified: Fri, 25 Sep 2020 23:48:02 GMT  
		Size: 118.1 KB (118072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ae72e7822ab820274e69307b627887e8b2dbd5a612eb37fbf340036a575f77`  
		Last Modified: Fri, 25 Sep 2020 23:48:03 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
