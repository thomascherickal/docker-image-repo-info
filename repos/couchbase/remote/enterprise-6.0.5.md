## `couchbase:enterprise-6.0.5`

```console
$ docker pull couchbase@sha256:9932059c3ef05613d0ad258913515f824df32c7cbc1dd8599a954c31fc6426ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:enterprise-6.0.5` - linux; amd64

```console
$ docker pull couchbase@sha256:d604760286cd1b0fc43da7c1b0ffe19ee46d69eb669eca5a949f889c6ec43ed6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **481.0 MB (481030036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17d958ecb35b69771c242140eabd73e26b87b746001b4f639bfecca4c4094c51`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Thu, 25 Mar 2021 22:33:52 GMT
ADD file:925571658dd8453e5c80d862f5791d6b26b3c2a8688937b11741f2f2c5cdbfd7 in / 
# Thu, 25 Mar 2021 22:33:53 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 25 Mar 2021 22:33:54 GMT
RUN rm -rf /var/lib/apt/lists/*
# Thu, 25 Mar 2021 22:33:55 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 25 Mar 2021 22:33:55 GMT
CMD ["/bin/bash"]
# Fri, 26 Mar 2021 10:21:26 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Fri, 26 Mar 2021 10:24:19 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 26 Mar 2021 10:24:20 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Fri, 26 Mar 2021 10:24:20 GMT
ARG CB_VERSION=6.0.5
# Fri, 26 Mar 2021 10:24:20 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5
# Fri, 26 Mar 2021 10:24:21 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu16.04_amd64.deb
# Fri, 26 Mar 2021 10:24:21 GMT
ARG CB_SHA256=3227bd9bf04affeea6c567a9e87cde585d2d49e5548b95204ffbda7dea8d451a
# Fri, 26 Mar 2021 10:24:21 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 26 Mar 2021 10:24:22 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=3227bd9bf04affeea6c567a9e87cde585d2d49e5548b95204ffbda7dea8d451a CB_VERSION=6.0.5
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 26 Mar 2021 10:25:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=3227bd9bf04affeea6c567a9e87cde585d2d49e5548b95204ffbda7dea8d451a CB_VERSION=6.0.5
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Fri, 26 Mar 2021 10:25:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=3227bd9bf04affeea6c567a9e87cde585d2d49e5548b95204ffbda7dea8d451a CB_VERSION=6.0.5
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 26 Mar 2021 10:25:13 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 26 Mar 2021 10:25:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=3227bd9bf04affeea6c567a9e87cde585d2d49e5548b95204ffbda7dea8d451a CB_VERSION=6.0.5
RUN chown -R couchbase:couchbase /etc/service
# Fri, 26 Mar 2021 10:25:15 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 26 Mar 2021 10:25:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=3227bd9bf04affeea6c567a9e87cde585d2d49e5548b95204ffbda7dea8d451a CB_VERSION=6.0.5
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 26 Mar 2021 10:25:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.5-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.5 CB_SHA256=3227bd9bf04affeea6c567a9e87cde585d2d49e5548b95204ffbda7dea8d451a CB_VERSION=6.0.5
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 26 Mar 2021 10:25:17 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 26 Mar 2021 10:25:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 26 Mar 2021 10:25:17 GMT
CMD ["couchbase-server"]
# Fri, 26 Mar 2021 10:25:17 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 26 Mar 2021 10:25:18 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:4007a89234b4f56c03e6831dc220550d2e5fba935d9f5f5bcea64857ac4f4888`  
		Last Modified: Mon, 18 Jan 2021 19:38:08 GMT  
		Size: 46.0 MB (45962352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1de0f9cdfc1f9f595acd2ea8724ea92a509d64a6936f0e645c65b504e7e4bc6`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 846.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ee6ca703b866ac2b74b6129d2db331936292f899e8e3a794474fdf81343605`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39e2761d3d4971e78914857af4c6bd9989873b53426cf2fef3e76983b166fa2`  
		Last Modified: Thu, 25 Mar 2021 22:36:02 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03230c57f910f142b80031a9ec258d69519b9559f760b0280984d9a2b179da2c`  
		Last Modified: Fri, 26 Mar 2021 10:30:52 GMT  
		Size: 14.3 MB (14298870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb608399ae4699b9010b2cc41b60c514cc9b02c82a411ec7cafcd0b5c5b3079d`  
		Last Modified: Fri, 26 Mar 2021 10:30:48 GMT  
		Size: 2.1 KB (2075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f0502c5b8b4075300d667861cff0218fbcd0adf6d765411cc64365b1cbda961`  
		Last Modified: Fri, 26 Mar 2021 10:31:40 GMT  
		Size: 420.6 MB (420642258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29bb22ab233a8a07cf928c2ae031b83f8f0d37f092a11a6630cfea84f0ceca5c`  
		Last Modified: Fri, 26 Mar 2021 10:30:48 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60e295d7671cd658281c87eef9e72bfb7d9541d74c5cf8a87a3dfbc61fd7ed8e`  
		Last Modified: Fri, 26 Mar 2021 10:30:48 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fab73fa5a9b8d93ef5b6f0642415b2c8e7647c12d77b030c6dcfcd9c642c08a`  
		Last Modified: Fri, 26 Mar 2021 10:30:45 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269b3a0d8f9bacbcf84312e6dd0e6d39cef5005e7221e05ff213ccefcee0c012`  
		Last Modified: Fri, 26 Mar 2021 10:30:45 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dd3c1a30fd2690d0b6d1935a9ed27e50f4955ad629abb303f11fb9dd42a54b2`  
		Last Modified: Fri, 26 Mar 2021 10:30:46 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a1de1306d42490f0c43747c94817d5f80622adb07a74a9020e89509f781b722`  
		Last Modified: Fri, 26 Mar 2021 10:30:46 GMT  
		Size: 120.6 KB (120601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742076bd9c0112c9922f9a5eee943e21d74d81d3206359e18f479acd8ab459fd`  
		Last Modified: Fri, 26 Mar 2021 10:30:46 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
