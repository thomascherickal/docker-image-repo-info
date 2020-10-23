<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchbase`

-	[`couchbase:6.0.4`](#couchbase604)
-	[`couchbase:6.6.0`](#couchbase660)
-	[`couchbase:community`](#couchbasecommunity)
-	[`couchbase:community-6.6.0`](#couchbasecommunity-660)
-	[`couchbase:enterprise`](#couchbaseenterprise)
-	[`couchbase:enterprise-6.0.4`](#couchbaseenterprise-604)
-	[`couchbase:enterprise-6.6.0`](#couchbaseenterprise-660)
-	[`couchbase:latest`](#couchbaselatest)

## `couchbase:6.0.4`

```console
$ docker pull couchbase@sha256:79d1cf371914ebf227a21b1eb2eee6ef680bff81c858cba7c29a0f509af9bd3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:6.0.4` - linux; amd64

```console
$ docker pull couchbase@sha256:cb11d88d090b7ff43dbff85412205809f2c55dd4aacdfd0e7f368de379b9bf0f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **481.9 MB (481935926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97945095546f6012f605429427e95586cb5b2753bcd2ff06ef0e6baac8f7f91d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:24:00 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Fri, 23 Oct 2020 18:26:41 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 23 Oct 2020 18:26:41 GMT
ARG CB_VERSION=6.0.4
# Fri, 23 Oct 2020 18:26:41 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4
# Fri, 23 Oct 2020 18:26:42 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb
# Fri, 23 Oct 2020 18:26:43 GMT
ARG CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf
# Fri, 23 Oct 2020 18:26:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 23 Oct 2020 18:26:49 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf CB_VERSION=6.0.4
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 23 Oct 2020 18:27:39 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf CB_VERSION=6.0.4
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Fri, 23 Oct 2020 18:27:39 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 23 Oct 2020 18:27:40 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf CB_VERSION=6.0.4
RUN chown -R couchbase:couchbase /etc/service
# Fri, 23 Oct 2020 18:27:40 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 23 Oct 2020 18:27:41 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf CB_VERSION=6.0.4
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 23 Oct 2020 18:27:42 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf CB_VERSION=6.0.4
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 23 Oct 2020 18:27:42 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 23 Oct 2020 18:27:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 23 Oct 2020 18:27:42 GMT
CMD ["couchbase-server"]
# Fri, 23 Oct 2020 18:27:42 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 23 Oct 2020 18:27:43 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf562855758bf55ae188a514cc224c00013dbce0e323191b4d4b989b8158413`  
		Last Modified: Fri, 23 Oct 2020 18:30:12 GMT  
		Size: 14.3 MB (14285721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8f3ff7c4cee3895db3136f95f2a4105e96abd43827cf03ddc3ce1f7a2e7e8f`  
		Last Modified: Fri, 23 Oct 2020 18:30:10 GMT  
		Size: 2.1 KB (2076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68d8cf695397c016d54332616f18c2421d73c6bcc677199d020a29f4cf39e00`  
		Last Modified: Fri, 23 Oct 2020 18:30:54 GMT  
		Size: 421.7 MB (421698144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508b27f5dedb0cfd2b35e37367eee6db5a5b1762fa660ceb4d6523a2d928ebf1`  
		Last Modified: Fri, 23 Oct 2020 18:30:09 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a78d424cdedf1a4e528624d00a70f0e8a426c86bf4f9191ac4c65c38e47bf1f`  
		Last Modified: Fri, 23 Oct 2020 18:30:06 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b4f2b630a5634f68d4c767d8c3cae2d5fdd6538c14242cf0a8f716441122aa`  
		Last Modified: Fri, 23 Oct 2020 18:30:06 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6e5d6236f1d30eed4e18abcde7ad54eba06865f7c5c1a38c67e5284a020e30`  
		Last Modified: Fri, 23 Oct 2020 18:30:07 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5824b441290447699b1e35c994ecc08197874c66f55d22f0b5b6c18f4912cfc`  
		Last Modified: Fri, 23 Oct 2020 18:30:06 GMT  
		Size: 120.6 KB (120598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8757bc850834bc436fe5567f57374ef72e79060c2d05ef192847b997508fa16b`  
		Last Modified: Fri, 23 Oct 2020 18:30:07 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:6.6.0`

```console
$ docker pull couchbase@sha256:1d811b3c382893f70f0cc0f2371a12d3671c1d5175bcc67e8c2a5c0bf4c8f976
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:6.6.0` - linux; amd64

```console
$ docker pull couchbase@sha256:029a3f91f2a2a4c471255670b5d6c9032836b80d0e1e62112e75d6754ed4c4dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **543.1 MB (543097083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64844065dcbc3d0a90c365c1f56421766a5cebf05f7ecbd3377af410fff09fd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:24:00 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Fri, 23 Oct 2020 18:24:15 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 23 Oct 2020 18:24:16 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Fri, 23 Oct 2020 18:24:16 GMT
ARG CB_VERSION=6.6.0
# Fri, 23 Oct 2020 18:24:16 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Fri, 23 Oct 2020 18:24:16 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb
# Fri, 23 Oct 2020 18:24:16 GMT
ARG CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9
# Fri, 23 Oct 2020 18:24:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 23 Oct 2020 18:24:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 23 Oct 2020 18:25:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Fri, 23 Oct 2020 18:25:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 23 Oct 2020 18:25:14 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 23 Oct 2020 18:25:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN chown -R couchbase:couchbase /etc/service
# Fri, 23 Oct 2020 18:25:15 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 23 Oct 2020 18:25:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 23 Oct 2020 18:25:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 23 Oct 2020 18:25:17 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 23 Oct 2020 18:25:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 23 Oct 2020 18:25:17 GMT
CMD ["couchbase-server"]
# Fri, 23 Oct 2020 18:25:17 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 23 Oct 2020 18:25:17 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c8f38d6e0af3267c209177ba2cacf7e1f63ce53fc5fb24e0aea5a3d30a7474`  
		Last Modified: Fri, 23 Oct 2020 18:28:08 GMT  
		Size: 5.8 MB (5827300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18d6f01cebdcc2467443ae6732abc383eec04e7367212a39e6d272812f72e94`  
		Last Modified: Fri, 23 Oct 2020 18:28:06 GMT  
		Size: 2.1 KB (2074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd039eadc80132f382154ff25165c9e58c3ba42b18a5acf2a925118af8bc78c`  
		Last Modified: Fri, 23 Oct 2020 18:29:07 GMT  
		Size: 491.3 MB (491320051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9b6ef215da2ed7609c8d650f50c40a2930edff5ba90c343ed58cd6f99e6ae8`  
		Last Modified: Fri, 23 Oct 2020 18:28:05 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e523c57bd123235dba6a4ee11a3c7f77da10774dbf1ee730b8433bf71af57e58`  
		Last Modified: Fri, 23 Oct 2020 18:28:05 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903f9f18b24b6a4ffa1d24ab2c92ee6264349a7c500551d5e39f97b9e4e66783`  
		Last Modified: Fri, 23 Oct 2020 18:28:03 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efb71e23d33ac0ce248884ec03301a74ea564752aa0c0d36f81321c13263e99`  
		Last Modified: Fri, 23 Oct 2020 18:28:04 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6c108820bbf03b95107a342e2ce980016f41a3f5fbcd5bf1ae90c293d5e878`  
		Last Modified: Fri, 23 Oct 2020 18:28:04 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e081344b802bd59f86bde4b88a210e223d724ebb78fee14d05ae1a8267378d`  
		Last Modified: Fri, 23 Oct 2020 18:28:03 GMT  
		Size: 118.1 KB (118076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52b41fe07ac144c268108187272cda92d188051c096078ab1c35bec8ee403bc`  
		Last Modified: Fri, 23 Oct 2020 18:28:04 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community`

```console
$ docker pull couchbase@sha256:4f2830c5850e0c4372b05b9fb452e161b3b2bda61963ed7d73a7213520646d55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:community` - linux; amd64

```console
$ docker pull couchbase@sha256:fd9876c944f380d553c9782b68a590e3f8cdeaa67ddf1f741e7430f0fde1c626
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.3 MB (371349559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:948d0290473b21f92cf588a14a833e7c610b4f532667ce8be0c8a0c89d14c3f2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:24:00 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Fri, 23 Oct 2020 18:24:15 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 23 Oct 2020 18:24:16 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Fri, 23 Oct 2020 18:24:16 GMT
ARG CB_VERSION=6.6.0
# Fri, 23 Oct 2020 18:24:16 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Fri, 23 Oct 2020 18:25:30 GMT
ARG CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb
# Fri, 23 Oct 2020 18:25:30 GMT
ARG CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e
# Fri, 23 Oct 2020 18:25:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 23 Oct 2020 18:25:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 23 Oct 2020 18:26:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Fri, 23 Oct 2020 18:26:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 23 Oct 2020 18:26:17 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 23 Oct 2020 18:26:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN chown -R couchbase:couchbase /etc/service
# Fri, 23 Oct 2020 18:26:18 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 23 Oct 2020 18:26:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 23 Oct 2020 18:26:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 23 Oct 2020 18:26:19 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 23 Oct 2020 18:26:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 23 Oct 2020 18:26:20 GMT
CMD ["couchbase-server"]
# Fri, 23 Oct 2020 18:26:20 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 23 Oct 2020 18:26:20 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c8f38d6e0af3267c209177ba2cacf7e1f63ce53fc5fb24e0aea5a3d30a7474`  
		Last Modified: Fri, 23 Oct 2020 18:28:08 GMT  
		Size: 5.8 MB (5827300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df891a1066d2e7baa5d06cf4fabcb06541cb750230c31d0a51f8b7b0d8f1dfcc`  
		Last Modified: Fri, 23 Oct 2020 18:29:18 GMT  
		Size: 2.1 KB (2079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498292b7b6009f59bd830a49c96a89a515950d3225cd39ccebf911626cc0f826`  
		Last Modified: Fri, 23 Oct 2020 18:29:58 GMT  
		Size: 319.6 MB (319572532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86277dc4a7fe631dacc7da67df1ea9a557364d911c9cf1e8a0de755e3ef72c0f`  
		Last Modified: Fri, 23 Oct 2020 18:29:17 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ccf2bb46bb331a32b67e4bf19d6e9d98ed5f8d649cb018e57ed2a5d89ddd6d`  
		Last Modified: Fri, 23 Oct 2020 18:29:17 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8730d27c152c1f06e8044065fa907fe4dfa501461fd6b6b6804e638b57be1fb8`  
		Last Modified: Fri, 23 Oct 2020 18:29:14 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebccfebf13e45ea69d05457122e66db22787ba3dd324d4dd0645a217586da60`  
		Last Modified: Fri, 23 Oct 2020 18:29:15 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12813b8c265dc79f760fa422b71bae701a3fa5a9c72c7d2df511f2b3960b9f15`  
		Last Modified: Fri, 23 Oct 2020 18:29:18 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816263bfaa80239953d7b462ab28fc0527cdd2c72b6d22c9060a75ddd91df853`  
		Last Modified: Fri, 23 Oct 2020 18:29:16 GMT  
		Size: 118.1 KB (118071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2493905ad452c83c80b5ef31f2bf2c6c2f33369a140c31a3b53127d27bb429`  
		Last Modified: Fri, 23 Oct 2020 18:29:15 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-6.6.0`

```console
$ docker pull couchbase@sha256:4f2830c5850e0c4372b05b9fb452e161b3b2bda61963ed7d73a7213520646d55
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:community-6.6.0` - linux; amd64

```console
$ docker pull couchbase@sha256:fd9876c944f380d553c9782b68a590e3f8cdeaa67ddf1f741e7430f0fde1c626
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.3 MB (371349559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:948d0290473b21f92cf588a14a833e7c610b4f532667ce8be0c8a0c89d14c3f2`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:24:00 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Fri, 23 Oct 2020 18:24:15 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 23 Oct 2020 18:24:16 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Fri, 23 Oct 2020 18:24:16 GMT
ARG CB_VERSION=6.6.0
# Fri, 23 Oct 2020 18:24:16 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Fri, 23 Oct 2020 18:25:30 GMT
ARG CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb
# Fri, 23 Oct 2020 18:25:30 GMT
ARG CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e
# Fri, 23 Oct 2020 18:25:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 23 Oct 2020 18:25:31 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 23 Oct 2020 18:26:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Fri, 23 Oct 2020 18:26:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 23 Oct 2020 18:26:17 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 23 Oct 2020 18:26:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN chown -R couchbase:couchbase /etc/service
# Fri, 23 Oct 2020 18:26:18 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 23 Oct 2020 18:26:18 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 23 Oct 2020 18:26:19 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=19ba0f8ac60fd63226c45674c3d113a91a0e9168787b38df59fec5e98d11257e CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 23 Oct 2020 18:26:19 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 23 Oct 2020 18:26:20 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 23 Oct 2020 18:26:20 GMT
CMD ["couchbase-server"]
# Fri, 23 Oct 2020 18:26:20 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 23 Oct 2020 18:26:20 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c8f38d6e0af3267c209177ba2cacf7e1f63ce53fc5fb24e0aea5a3d30a7474`  
		Last Modified: Fri, 23 Oct 2020 18:28:08 GMT  
		Size: 5.8 MB (5827300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df891a1066d2e7baa5d06cf4fabcb06541cb750230c31d0a51f8b7b0d8f1dfcc`  
		Last Modified: Fri, 23 Oct 2020 18:29:18 GMT  
		Size: 2.1 KB (2079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:498292b7b6009f59bd830a49c96a89a515950d3225cd39ccebf911626cc0f826`  
		Last Modified: Fri, 23 Oct 2020 18:29:58 GMT  
		Size: 319.6 MB (319572532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86277dc4a7fe631dacc7da67df1ea9a557364d911c9cf1e8a0de755e3ef72c0f`  
		Last Modified: Fri, 23 Oct 2020 18:29:17 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ccf2bb46bb331a32b67e4bf19d6e9d98ed5f8d649cb018e57ed2a5d89ddd6d`  
		Last Modified: Fri, 23 Oct 2020 18:29:17 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8730d27c152c1f06e8044065fa907fe4dfa501461fd6b6b6804e638b57be1fb8`  
		Last Modified: Fri, 23 Oct 2020 18:29:14 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ebccfebf13e45ea69d05457122e66db22787ba3dd324d4dd0645a217586da60`  
		Last Modified: Fri, 23 Oct 2020 18:29:15 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12813b8c265dc79f760fa422b71bae701a3fa5a9c72c7d2df511f2b3960b9f15`  
		Last Modified: Fri, 23 Oct 2020 18:29:18 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816263bfaa80239953d7b462ab28fc0527cdd2c72b6d22c9060a75ddd91df853`  
		Last Modified: Fri, 23 Oct 2020 18:29:16 GMT  
		Size: 118.1 KB (118071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2493905ad452c83c80b5ef31f2bf2c6c2f33369a140c31a3b53127d27bb429`  
		Last Modified: Fri, 23 Oct 2020 18:29:15 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise`

```console
$ docker pull couchbase@sha256:1d811b3c382893f70f0cc0f2371a12d3671c1d5175bcc67e8c2a5c0bf4c8f976
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:enterprise` - linux; amd64

```console
$ docker pull couchbase@sha256:029a3f91f2a2a4c471255670b5d6c9032836b80d0e1e62112e75d6754ed4c4dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **543.1 MB (543097083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64844065dcbc3d0a90c365c1f56421766a5cebf05f7ecbd3377af410fff09fd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:24:00 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Fri, 23 Oct 2020 18:24:15 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 23 Oct 2020 18:24:16 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Fri, 23 Oct 2020 18:24:16 GMT
ARG CB_VERSION=6.6.0
# Fri, 23 Oct 2020 18:24:16 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Fri, 23 Oct 2020 18:24:16 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb
# Fri, 23 Oct 2020 18:24:16 GMT
ARG CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9
# Fri, 23 Oct 2020 18:24:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 23 Oct 2020 18:24:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 23 Oct 2020 18:25:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Fri, 23 Oct 2020 18:25:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 23 Oct 2020 18:25:14 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 23 Oct 2020 18:25:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN chown -R couchbase:couchbase /etc/service
# Fri, 23 Oct 2020 18:25:15 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 23 Oct 2020 18:25:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 23 Oct 2020 18:25:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 23 Oct 2020 18:25:17 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 23 Oct 2020 18:25:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 23 Oct 2020 18:25:17 GMT
CMD ["couchbase-server"]
# Fri, 23 Oct 2020 18:25:17 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 23 Oct 2020 18:25:17 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c8f38d6e0af3267c209177ba2cacf7e1f63ce53fc5fb24e0aea5a3d30a7474`  
		Last Modified: Fri, 23 Oct 2020 18:28:08 GMT  
		Size: 5.8 MB (5827300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18d6f01cebdcc2467443ae6732abc383eec04e7367212a39e6d272812f72e94`  
		Last Modified: Fri, 23 Oct 2020 18:28:06 GMT  
		Size: 2.1 KB (2074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd039eadc80132f382154ff25165c9e58c3ba42b18a5acf2a925118af8bc78c`  
		Last Modified: Fri, 23 Oct 2020 18:29:07 GMT  
		Size: 491.3 MB (491320051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9b6ef215da2ed7609c8d650f50c40a2930edff5ba90c343ed58cd6f99e6ae8`  
		Last Modified: Fri, 23 Oct 2020 18:28:05 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e523c57bd123235dba6a4ee11a3c7f77da10774dbf1ee730b8433bf71af57e58`  
		Last Modified: Fri, 23 Oct 2020 18:28:05 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903f9f18b24b6a4ffa1d24ab2c92ee6264349a7c500551d5e39f97b9e4e66783`  
		Last Modified: Fri, 23 Oct 2020 18:28:03 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efb71e23d33ac0ce248884ec03301a74ea564752aa0c0d36f81321c13263e99`  
		Last Modified: Fri, 23 Oct 2020 18:28:04 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6c108820bbf03b95107a342e2ce980016f41a3f5fbcd5bf1ae90c293d5e878`  
		Last Modified: Fri, 23 Oct 2020 18:28:04 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e081344b802bd59f86bde4b88a210e223d724ebb78fee14d05ae1a8267378d`  
		Last Modified: Fri, 23 Oct 2020 18:28:03 GMT  
		Size: 118.1 KB (118076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52b41fe07ac144c268108187272cda92d188051c096078ab1c35bec8ee403bc`  
		Last Modified: Fri, 23 Oct 2020 18:28:04 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.0.4`

```console
$ docker pull couchbase@sha256:79d1cf371914ebf227a21b1eb2eee6ef680bff81c858cba7c29a0f509af9bd3d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:enterprise-6.0.4` - linux; amd64

```console
$ docker pull couchbase@sha256:cb11d88d090b7ff43dbff85412205809f2c55dd4aacdfd0e7f368de379b9bf0f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **481.9 MB (481935926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97945095546f6012f605429427e95586cb5b2753bcd2ff06ef0e6baac8f7f91d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:24:00 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Fri, 23 Oct 2020 18:26:41 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 23 Oct 2020 18:26:41 GMT
ARG CB_VERSION=6.0.4
# Fri, 23 Oct 2020 18:26:41 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4
# Fri, 23 Oct 2020 18:26:42 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb
# Fri, 23 Oct 2020 18:26:43 GMT
ARG CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf
# Fri, 23 Oct 2020 18:26:44 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 23 Oct 2020 18:26:49 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf CB_VERSION=6.0.4
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 23 Oct 2020 18:27:39 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf CB_VERSION=6.0.4
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Fri, 23 Oct 2020 18:27:39 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 23 Oct 2020 18:27:40 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf CB_VERSION=6.0.4
RUN chown -R couchbase:couchbase /etc/service
# Fri, 23 Oct 2020 18:27:40 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 23 Oct 2020 18:27:41 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf CB_VERSION=6.0.4
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 23 Oct 2020 18:27:42 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.0.4-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.4 CB_SHA256=a9144e41fdb62dc872e09be617f69157f23568cc6e1d425e7adaf580aeba9adf CB_VERSION=6.0.4
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 23 Oct 2020 18:27:42 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 23 Oct 2020 18:27:42 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 23 Oct 2020 18:27:42 GMT
CMD ["couchbase-server"]
# Fri, 23 Oct 2020 18:27:42 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 23 Oct 2020 18:27:43 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faf562855758bf55ae188a514cc224c00013dbce0e323191b4d4b989b8158413`  
		Last Modified: Fri, 23 Oct 2020 18:30:12 GMT  
		Size: 14.3 MB (14285721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd8f3ff7c4cee3895db3136f95f2a4105e96abd43827cf03ddc3ce1f7a2e7e8f`  
		Last Modified: Fri, 23 Oct 2020 18:30:10 GMT  
		Size: 2.1 KB (2076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f68d8cf695397c016d54332616f18c2421d73c6bcc677199d020a29f4cf39e00`  
		Last Modified: Fri, 23 Oct 2020 18:30:54 GMT  
		Size: 421.7 MB (421698144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:508b27f5dedb0cfd2b35e37367eee6db5a5b1762fa660ceb4d6523a2d928ebf1`  
		Last Modified: Fri, 23 Oct 2020 18:30:09 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a78d424cdedf1a4e528624d00a70f0e8a426c86bf4f9191ac4c65c38e47bf1f`  
		Last Modified: Fri, 23 Oct 2020 18:30:06 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b4f2b630a5634f68d4c767d8c3cae2d5fdd6538c14242cf0a8f716441122aa`  
		Last Modified: Fri, 23 Oct 2020 18:30:06 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6e5d6236f1d30eed4e18abcde7ad54eba06865f7c5c1a38c67e5284a020e30`  
		Last Modified: Fri, 23 Oct 2020 18:30:07 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5824b441290447699b1e35c994ecc08197874c66f55d22f0b5b6c18f4912cfc`  
		Last Modified: Fri, 23 Oct 2020 18:30:06 GMT  
		Size: 120.6 KB (120598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8757bc850834bc436fe5567f57374ef72e79060c2d05ef192847b997508fa16b`  
		Last Modified: Fri, 23 Oct 2020 18:30:07 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.6.0`

```console
$ docker pull couchbase@sha256:1d811b3c382893f70f0cc0f2371a12d3671c1d5175bcc67e8c2a5c0bf4c8f976
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:enterprise-6.6.0` - linux; amd64

```console
$ docker pull couchbase@sha256:029a3f91f2a2a4c471255670b5d6c9032836b80d0e1e62112e75d6754ed4c4dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **543.1 MB (543097083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64844065dcbc3d0a90c365c1f56421766a5cebf05f7ecbd3377af410fff09fd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:24:00 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Fri, 23 Oct 2020 18:24:15 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 23 Oct 2020 18:24:16 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Fri, 23 Oct 2020 18:24:16 GMT
ARG CB_VERSION=6.6.0
# Fri, 23 Oct 2020 18:24:16 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Fri, 23 Oct 2020 18:24:16 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb
# Fri, 23 Oct 2020 18:24:16 GMT
ARG CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9
# Fri, 23 Oct 2020 18:24:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 23 Oct 2020 18:24:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 23 Oct 2020 18:25:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Fri, 23 Oct 2020 18:25:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 23 Oct 2020 18:25:14 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 23 Oct 2020 18:25:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN chown -R couchbase:couchbase /etc/service
# Fri, 23 Oct 2020 18:25:15 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 23 Oct 2020 18:25:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 23 Oct 2020 18:25:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 23 Oct 2020 18:25:17 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 23 Oct 2020 18:25:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 23 Oct 2020 18:25:17 GMT
CMD ["couchbase-server"]
# Fri, 23 Oct 2020 18:25:17 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 23 Oct 2020 18:25:17 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c8f38d6e0af3267c209177ba2cacf7e1f63ce53fc5fb24e0aea5a3d30a7474`  
		Last Modified: Fri, 23 Oct 2020 18:28:08 GMT  
		Size: 5.8 MB (5827300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18d6f01cebdcc2467443ae6732abc383eec04e7367212a39e6d272812f72e94`  
		Last Modified: Fri, 23 Oct 2020 18:28:06 GMT  
		Size: 2.1 KB (2074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd039eadc80132f382154ff25165c9e58c3ba42b18a5acf2a925118af8bc78c`  
		Last Modified: Fri, 23 Oct 2020 18:29:07 GMT  
		Size: 491.3 MB (491320051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9b6ef215da2ed7609c8d650f50c40a2930edff5ba90c343ed58cd6f99e6ae8`  
		Last Modified: Fri, 23 Oct 2020 18:28:05 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e523c57bd123235dba6a4ee11a3c7f77da10774dbf1ee730b8433bf71af57e58`  
		Last Modified: Fri, 23 Oct 2020 18:28:05 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903f9f18b24b6a4ffa1d24ab2c92ee6264349a7c500551d5e39f97b9e4e66783`  
		Last Modified: Fri, 23 Oct 2020 18:28:03 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efb71e23d33ac0ce248884ec03301a74ea564752aa0c0d36f81321c13263e99`  
		Last Modified: Fri, 23 Oct 2020 18:28:04 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6c108820bbf03b95107a342e2ce980016f41a3f5fbcd5bf1ae90c293d5e878`  
		Last Modified: Fri, 23 Oct 2020 18:28:04 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e081344b802bd59f86bde4b88a210e223d724ebb78fee14d05ae1a8267378d`  
		Last Modified: Fri, 23 Oct 2020 18:28:03 GMT  
		Size: 118.1 KB (118076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52b41fe07ac144c268108187272cda92d188051c096078ab1c35bec8ee403bc`  
		Last Modified: Fri, 23 Oct 2020 18:28:04 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:latest`

```console
$ docker pull couchbase@sha256:1d811b3c382893f70f0cc0f2371a12d3671c1d5175bcc67e8c2a5c0bf4c8f976
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:latest` - linux; amd64

```console
$ docker pull couchbase@sha256:029a3f91f2a2a4c471255670b5d6c9032836b80d0e1e62112e75d6754ed4c4dc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **543.1 MB (543097083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c64844065dcbc3d0a90c365c1f56421766a5cebf05f7ecbd3377af410fff09fd`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 23 Oct 2020 17:33:08 GMT
ADD file:c1f3147c7b6710af5affd417ff822ee28df872d716003858d3d2e23d2277c981 in / 
# Fri, 23 Oct 2020 17:33:09 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 23 Oct 2020 17:33:09 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 23 Oct 2020 17:33:10 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 23 Oct 2020 17:33:10 GMT
CMD ["/bin/bash"]
# Fri, 23 Oct 2020 18:24:00 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Fri, 23 Oct 2020 18:24:15 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 23 Oct 2020 18:24:16 GMT
RUN if [ ! -x /usr/sbin/runsvdir-start ]; then         cp -a /etc/runit/2 /usr/sbin/runsvdir-start;     fi
# Fri, 23 Oct 2020 18:24:16 GMT
ARG CB_VERSION=6.6.0
# Fri, 23 Oct 2020 18:24:16 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0
# Fri, 23 Oct 2020 18:24:16 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb
# Fri, 23 Oct 2020 18:24:16 GMT
ARG CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9
# Fri, 23 Oct 2020 18:24:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 23 Oct 2020 18:24:17 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 23 Oct 2020 18:25:13 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Fri, 23 Oct 2020 18:25:14 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Fri, 23 Oct 2020 18:25:14 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 23 Oct 2020 18:25:15 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN chown -R couchbase:couchbase /etc/service
# Fri, 23 Oct 2020 18:25:15 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 23 Oct 2020 18:25:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 23 Oct 2020 18:25:16 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.6.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.6.0 CB_SHA256=9f666b2e39c11b17a9cc74c00967d97efeab08e23b93e8bbdec582ce009c65c9 CB_VERSION=6.6.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 23 Oct 2020 18:25:17 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 23 Oct 2020 18:25:17 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 23 Oct 2020 18:25:17 GMT
CMD ["couchbase-server"]
# Fri, 23 Oct 2020 18:25:17 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 23 Oct 2020 18:25:17 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:2c11b7cecaa5d3e2a57e290921ababbfb8572b549015168d4cbd91c340d2c566`  
		Last Modified: Wed, 14 Oct 2020 13:20:30 GMT  
		Size: 45.8 MB (45825714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04637fa562525a9366f00e8f4b08d04a347bded1ee513738451ef9d42b4dfc4e`  
		Last Modified: Fri, 23 Oct 2020 17:33:48 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6e6af23a0f38c4a6511147d2a9dc06a07a7afa0669000cb62720c7eafe031ae`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a424de92ad71639c5cabadcdab0493e4067eb2f9cf109ffef40db178349238`  
		Last Modified: Fri, 23 Oct 2020 17:33:49 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c8f38d6e0af3267c209177ba2cacf7e1f63ce53fc5fb24e0aea5a3d30a7474`  
		Last Modified: Fri, 23 Oct 2020 18:28:08 GMT  
		Size: 5.8 MB (5827300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e18d6f01cebdcc2467443ae6732abc383eec04e7367212a39e6d272812f72e94`  
		Last Modified: Fri, 23 Oct 2020 18:28:06 GMT  
		Size: 2.1 KB (2074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd039eadc80132f382154ff25165c9e58c3ba42b18a5acf2a925118af8bc78c`  
		Last Modified: Fri, 23 Oct 2020 18:29:07 GMT  
		Size: 491.3 MB (491320051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9b6ef215da2ed7609c8d650f50c40a2930edff5ba90c343ed58cd6f99e6ae8`  
		Last Modified: Fri, 23 Oct 2020 18:28:05 GMT  
		Size: 192.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e523c57bd123235dba6a4ee11a3c7f77da10774dbf1ee730b8433bf71af57e58`  
		Last Modified: Fri, 23 Oct 2020 18:28:05 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:903f9f18b24b6a4ffa1d24ab2c92ee6264349a7c500551d5e39f97b9e4e66783`  
		Last Modified: Fri, 23 Oct 2020 18:28:03 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efb71e23d33ac0ce248884ec03301a74ea564752aa0c0d36f81321c13263e99`  
		Last Modified: Fri, 23 Oct 2020 18:28:04 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6c108820bbf03b95107a342e2ce980016f41a3f5fbcd5bf1ae90c293d5e878`  
		Last Modified: Fri, 23 Oct 2020 18:28:04 GMT  
		Size: 215.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e081344b802bd59f86bde4b88a210e223d724ebb78fee14d05ae1a8267378d`  
		Last Modified: Fri, 23 Oct 2020 18:28:03 GMT  
		Size: 118.1 KB (118076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e52b41fe07ac144c268108187272cda92d188051c096078ab1c35bec8ee403bc`  
		Last Modified: Fri, 23 Oct 2020 18:28:04 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
