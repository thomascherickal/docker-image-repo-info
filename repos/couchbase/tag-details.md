<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `couchbase`

-	[`couchbase:6.5.0`](#couchbase650)
-	[`couchbase:community`](#couchbasecommunity)
-	[`couchbase:community-6.5.0`](#couchbasecommunity-650)
-	[`couchbase:enterprise`](#couchbaseenterprise)
-	[`couchbase:enterprise-6.5.0`](#couchbaseenterprise-650)
-	[`couchbase:latest`](#couchbaselatest)

## `couchbase:6.5.0`

```console
$ docker pull couchbase@sha256:3aeadfedfca245d9c17ab114087fd9d24f01d47046add5d8e18638fffb6c3b63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:6.5.0` - linux; amd64

```console
$ docker pull couchbase@sha256:7cf84db2e211583ec1ce83eb46deac35849d7c91380f7e79b5e1ac211629684e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **556.0 MB (555975314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5da7e004db8c0f1e870f1205e54beef15cb38ff1144e223573293bd99665a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:21:52 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Fri, 21 Feb 2020 23:22:08 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 21 Feb 2020 23:22:08 GMT
ARG CB_VERSION=6.5.0
# Fri, 21 Feb 2020 23:22:09 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0
# Fri, 21 Feb 2020 23:22:09 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb
# Fri, 21 Feb 2020 23:22:09 GMT
ARG CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b
# Fri, 21 Feb 2020 23:22:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 21 Feb 2020 23:22:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b CB_VERSION=6.5.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 21 Feb 2020 23:23:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b CB_VERSION=6.5.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Fri, 21 Feb 2020 23:23:05 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 21 Feb 2020 23:23:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b CB_VERSION=6.5.0
RUN chown -R couchbase:couchbase /etc/service
# Fri, 21 Feb 2020 23:23:06 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 21 Feb 2020 23:23:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b CB_VERSION=6.5.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 21 Feb 2020 23:23:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b CB_VERSION=6.5.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 21 Feb 2020 23:23:08 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 21 Feb 2020 23:23:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Feb 2020 23:23:08 GMT
CMD ["couchbase-server"]
# Fri, 21 Feb 2020 23:23:08 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 21 Feb 2020 23:23:08 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37acf92bdab20e91916c20a5968e5cb55bcec6d8043d20d2d27ae940ae34295b`  
		Last Modified: Fri, 21 Feb 2020 23:24:20 GMT  
		Size: 5.9 MB (5853564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10cf7308a312b01ad29f3f16409e364a3b34aea3851e261329323c3781752721`  
		Last Modified: Fri, 21 Feb 2020 23:24:19 GMT  
		Size: 2.1 KB (2081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45a9b3e71d633ebcbc6710221ff737e0c62018e010599f198b986e8b5884e3e`  
		Last Modified: Fri, 21 Feb 2020 23:25:18 GMT  
		Size: 505.8 MB (505806202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33af0d5a0317b1e1e74f02478f15a311677873bce21048f8b769419ff529b9d8`  
		Last Modified: Fri, 21 Feb 2020 23:24:19 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20304ddc237219a10e926344052e99e6fd41d2607651f44bbc2d56061b6b46f7`  
		Last Modified: Fri, 21 Feb 2020 23:24:17 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d5c28589d3b2def6eb96123639d8150cdbf73f17fbcdf3b1e38d8cae058499`  
		Last Modified: Fri, 21 Feb 2020 23:24:18 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50435a6426b6a1b0b3972af671594ec5666a008e3afffc1b1b22818b2039723d`  
		Last Modified: Fri, 21 Feb 2020 23:24:18 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a41097a0fbceab6d0bae1b81e7310b93de80b0d734d9dd56eced0fab028c0c`  
		Last Modified: Fri, 21 Feb 2020 23:24:18 GMT  
		Size: 118.1 KB (118066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4416145aaa814cce0a7e06b2c85f524f18fda317ad66a427f845d80f94ce1a2f`  
		Last Modified: Fri, 21 Feb 2020 23:24:18 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community`

```console
$ docker pull couchbase@sha256:a9fd5dc275e4f401016bfdffe3cda77a27cfe835b1f3271ef1421c1ae9f41726
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:community` - linux; amd64

```console
$ docker pull couchbase@sha256:562c577b21b7876a5bd2d34855c4cdb4b818ce608f3fbcc73ba374efffb49bb4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.5 MB (199536655 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d4122aca7c16ae7863b0b21909848c7054e22c29fcdb17887b2cf57b0d4e714`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:21:52 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Fri, 21 Feb 2020 23:23:38 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl python-httplib2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 21 Feb 2020 23:23:41 GMT
ARG CB_VERSION=6.0.0
# Fri, 21 Feb 2020 23:23:42 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.0
# Fri, 21 Feb 2020 23:23:42 GMT
ARG CB_PACKAGE=couchbase-server-community_6.0.0-ubuntu16.04_amd64.deb
# Fri, 21 Feb 2020 23:23:43 GMT
ARG CB_SHA256=949b1ded72776a557b9cd3ac89253a4fe6aed079966a4057c5aec41ae5a30ece
# Fri, 21 Feb 2020 23:23:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 21 Feb 2020 23:23:44 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.0.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.0 CB_SHA256=949b1ded72776a557b9cd3ac89253a4fe6aed079966a4057c5aec41ae5a30ece CB_VERSION=6.0.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 21 Feb 2020 23:23:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.0.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.0 CB_SHA256=949b1ded72776a557b9cd3ac89253a4fe6aed079966a4057c5aec41ae5a30ece CB_VERSION=6.0.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Fri, 21 Feb 2020 23:24:00 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 21 Feb 2020 23:24:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.0.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.0 CB_SHA256=949b1ded72776a557b9cd3ac89253a4fe6aed079966a4057c5aec41ae5a30ece CB_VERSION=6.0.0
RUN chown -R couchbase:couchbase /etc/service
# Fri, 21 Feb 2020 23:24:01 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 21 Feb 2020 23:24:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.0.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.0 CB_SHA256=949b1ded72776a557b9cd3ac89253a4fe6aed079966a4057c5aec41ae5a30ece CB_VERSION=6.0.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 21 Feb 2020 23:24:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-community_6.0.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.0.0 CB_SHA256=949b1ded72776a557b9cd3ac89253a4fe6aed079966a4057c5aec41ae5a30ece CB_VERSION=6.0.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 21 Feb 2020 23:24:03 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 21 Feb 2020 23:24:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Feb 2020 23:24:03 GMT
CMD ["couchbase-server"]
# Fri, 21 Feb 2020 23:24:03 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 21 Feb 2020 23:24:03 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b052b8d2b896b39f83ddaf7afc8682af0526601ed145b1ebebda5892d866b67`  
		Last Modified: Fri, 21 Feb 2020 23:25:30 GMT  
		Size: 14.3 MB (14330790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bedaefc2f1b2e8bd2ad00c4a02c192edbf87a4ac4a5c11680f506f608ebbf7de`  
		Last Modified: Fri, 21 Feb 2020 23:25:26 GMT  
		Size: 2.1 KB (2080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f38b56650b9caa4a9fce1848ed4520f14ba25212aec4edf914bebd69516ad5`  
		Last Modified: Fri, 21 Feb 2020 23:25:48 GMT  
		Size: 140.9 MB (140887793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6623d57dfa3939320cb4f036b6505534a28e02fca54b5c6ae47a9176dbcf875`  
		Last Modified: Fri, 21 Feb 2020 23:25:26 GMT  
		Size: 404.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f219a8f4769baa9670b47cd8f3c2c1c3783d88c1d69aac86c07d66ee7e8f6daf`  
		Last Modified: Fri, 21 Feb 2020 23:25:25 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93e29ae9cc33d1e7cf23a4b881aafab5fd2d5b15f6f5a6b483055c8e0bf4f08`  
		Last Modified: Fri, 21 Feb 2020 23:25:25 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32c577d573a4d4d96bfb451282428f1bae58fe2b84ba24f0e95a485bc6ad7af`  
		Last Modified: Fri, 21 Feb 2020 23:25:25 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244aa8e60a0857a81015fbd17fbc7e7c134c7f4b584b997596876c368ed3e9dd`  
		Last Modified: Fri, 21 Feb 2020 23:25:25 GMT  
		Size: 120.6 KB (120597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c891635290eaed1c9bee26b8c5fe62e94a4ba3897aeb8f7429c9f5d17f6fa3`  
		Last Modified: Fri, 21 Feb 2020 23:25:25 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:community-6.5.0`

**does not exist** (yet?)

## `couchbase:enterprise`

```console
$ docker pull couchbase@sha256:3aeadfedfca245d9c17ab114087fd9d24f01d47046add5d8e18638fffb6c3b63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:enterprise` - linux; amd64

```console
$ docker pull couchbase@sha256:7cf84db2e211583ec1ce83eb46deac35849d7c91380f7e79b5e1ac211629684e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **556.0 MB (555975314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5da7e004db8c0f1e870f1205e54beef15cb38ff1144e223573293bd99665a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:21:52 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Fri, 21 Feb 2020 23:22:08 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 21 Feb 2020 23:22:08 GMT
ARG CB_VERSION=6.5.0
# Fri, 21 Feb 2020 23:22:09 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0
# Fri, 21 Feb 2020 23:22:09 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb
# Fri, 21 Feb 2020 23:22:09 GMT
ARG CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b
# Fri, 21 Feb 2020 23:22:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 21 Feb 2020 23:22:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b CB_VERSION=6.5.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 21 Feb 2020 23:23:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b CB_VERSION=6.5.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Fri, 21 Feb 2020 23:23:05 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 21 Feb 2020 23:23:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b CB_VERSION=6.5.0
RUN chown -R couchbase:couchbase /etc/service
# Fri, 21 Feb 2020 23:23:06 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 21 Feb 2020 23:23:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b CB_VERSION=6.5.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 21 Feb 2020 23:23:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b CB_VERSION=6.5.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 21 Feb 2020 23:23:08 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 21 Feb 2020 23:23:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Feb 2020 23:23:08 GMT
CMD ["couchbase-server"]
# Fri, 21 Feb 2020 23:23:08 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 21 Feb 2020 23:23:08 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37acf92bdab20e91916c20a5968e5cb55bcec6d8043d20d2d27ae940ae34295b`  
		Last Modified: Fri, 21 Feb 2020 23:24:20 GMT  
		Size: 5.9 MB (5853564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10cf7308a312b01ad29f3f16409e364a3b34aea3851e261329323c3781752721`  
		Last Modified: Fri, 21 Feb 2020 23:24:19 GMT  
		Size: 2.1 KB (2081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45a9b3e71d633ebcbc6710221ff737e0c62018e010599f198b986e8b5884e3e`  
		Last Modified: Fri, 21 Feb 2020 23:25:18 GMT  
		Size: 505.8 MB (505806202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33af0d5a0317b1e1e74f02478f15a311677873bce21048f8b769419ff529b9d8`  
		Last Modified: Fri, 21 Feb 2020 23:24:19 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20304ddc237219a10e926344052e99e6fd41d2607651f44bbc2d56061b6b46f7`  
		Last Modified: Fri, 21 Feb 2020 23:24:17 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d5c28589d3b2def6eb96123639d8150cdbf73f17fbcdf3b1e38d8cae058499`  
		Last Modified: Fri, 21 Feb 2020 23:24:18 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50435a6426b6a1b0b3972af671594ec5666a008e3afffc1b1b22818b2039723d`  
		Last Modified: Fri, 21 Feb 2020 23:24:18 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a41097a0fbceab6d0bae1b81e7310b93de80b0d734d9dd56eced0fab028c0c`  
		Last Modified: Fri, 21 Feb 2020 23:24:18 GMT  
		Size: 118.1 KB (118066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4416145aaa814cce0a7e06b2c85f524f18fda317ad66a427f845d80f94ce1a2f`  
		Last Modified: Fri, 21 Feb 2020 23:24:18 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:enterprise-6.5.0`

```console
$ docker pull couchbase@sha256:3aeadfedfca245d9c17ab114087fd9d24f01d47046add5d8e18638fffb6c3b63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:enterprise-6.5.0` - linux; amd64

```console
$ docker pull couchbase@sha256:7cf84db2e211583ec1ce83eb46deac35849d7c91380f7e79b5e1ac211629684e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **556.0 MB (555975314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5da7e004db8c0f1e870f1205e54beef15cb38ff1144e223573293bd99665a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:21:52 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Fri, 21 Feb 2020 23:22:08 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 21 Feb 2020 23:22:08 GMT
ARG CB_VERSION=6.5.0
# Fri, 21 Feb 2020 23:22:09 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0
# Fri, 21 Feb 2020 23:22:09 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb
# Fri, 21 Feb 2020 23:22:09 GMT
ARG CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b
# Fri, 21 Feb 2020 23:22:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 21 Feb 2020 23:22:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b CB_VERSION=6.5.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 21 Feb 2020 23:23:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b CB_VERSION=6.5.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Fri, 21 Feb 2020 23:23:05 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 21 Feb 2020 23:23:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b CB_VERSION=6.5.0
RUN chown -R couchbase:couchbase /etc/service
# Fri, 21 Feb 2020 23:23:06 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 21 Feb 2020 23:23:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b CB_VERSION=6.5.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 21 Feb 2020 23:23:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b CB_VERSION=6.5.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 21 Feb 2020 23:23:08 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 21 Feb 2020 23:23:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Feb 2020 23:23:08 GMT
CMD ["couchbase-server"]
# Fri, 21 Feb 2020 23:23:08 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 21 Feb 2020 23:23:08 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37acf92bdab20e91916c20a5968e5cb55bcec6d8043d20d2d27ae940ae34295b`  
		Last Modified: Fri, 21 Feb 2020 23:24:20 GMT  
		Size: 5.9 MB (5853564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10cf7308a312b01ad29f3f16409e364a3b34aea3851e261329323c3781752721`  
		Last Modified: Fri, 21 Feb 2020 23:24:19 GMT  
		Size: 2.1 KB (2081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45a9b3e71d633ebcbc6710221ff737e0c62018e010599f198b986e8b5884e3e`  
		Last Modified: Fri, 21 Feb 2020 23:25:18 GMT  
		Size: 505.8 MB (505806202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33af0d5a0317b1e1e74f02478f15a311677873bce21048f8b769419ff529b9d8`  
		Last Modified: Fri, 21 Feb 2020 23:24:19 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20304ddc237219a10e926344052e99e6fd41d2607651f44bbc2d56061b6b46f7`  
		Last Modified: Fri, 21 Feb 2020 23:24:17 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d5c28589d3b2def6eb96123639d8150cdbf73f17fbcdf3b1e38d8cae058499`  
		Last Modified: Fri, 21 Feb 2020 23:24:18 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50435a6426b6a1b0b3972af671594ec5666a008e3afffc1b1b22818b2039723d`  
		Last Modified: Fri, 21 Feb 2020 23:24:18 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a41097a0fbceab6d0bae1b81e7310b93de80b0d734d9dd56eced0fab028c0c`  
		Last Modified: Fri, 21 Feb 2020 23:24:18 GMT  
		Size: 118.1 KB (118066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4416145aaa814cce0a7e06b2c85f524f18fda317ad66a427f845d80f94ce1a2f`  
		Last Modified: Fri, 21 Feb 2020 23:24:18 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `couchbase:latest`

```console
$ docker pull couchbase@sha256:3aeadfedfca245d9c17ab114087fd9d24f01d47046add5d8e18638fffb6c3b63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:latest` - linux; amd64

```console
$ docker pull couchbase@sha256:7cf84db2e211583ec1ce83eb46deac35849d7c91380f7e79b5e1ac211629684e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **556.0 MB (555975314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe5da7e004db8c0f1e870f1205e54beef15cb38ff1144e223573293bd99665a7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["couchbase-server"]`

```dockerfile
# Fri, 21 Feb 2020 22:22:27 GMT
ADD file:1f70668251e2e58cee0ff0c22ee805f8a269ac6f8934c07f7e89dca6cc1de3aa in / 
# Fri, 21 Feb 2020 22:22:27 GMT
RUN rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:22:28 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:22:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:22:30 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:21:52 GMT
MAINTAINER Couchbase Docker Team <docker@couchbase.com>
# Fri, 21 Feb 2020 23:22:08 GMT
RUN apt-get update &&     apt-get install -yq runit wget chrpath tzdata     lsof lshw sysstat net-tools numactl bzip2 &&     apt-get autoremove && apt-get clean &&     rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
# Fri, 21 Feb 2020 23:22:08 GMT
ARG CB_VERSION=6.5.0
# Fri, 21 Feb 2020 23:22:09 GMT
ARG CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0
# Fri, 21 Feb 2020 23:22:09 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb
# Fri, 21 Feb 2020 23:22:09 GMT
ARG CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b
# Fri, 21 Feb 2020 23:22:09 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Fri, 21 Feb 2020 23:22:10 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b CB_VERSION=6.5.0
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Fri, 21 Feb 2020 23:23:05 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b CB_VERSION=6.5.0
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Fri, 21 Feb 2020 23:23:05 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Fri, 21 Feb 2020 23:23:06 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b CB_VERSION=6.5.0
RUN chown -R couchbase:couchbase /etc/service
# Fri, 21 Feb 2020 23:23:06 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Fri, 21 Feb 2020 23:23:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b CB_VERSION=6.5.0
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Fri, 21 Feb 2020 23:23:07 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_6.5.0-ubuntu16.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/6.5.0 CB_SHA256=5505c6bb026090dae7351e9d83caeab00437f19e48e826afd4cb6bafc484cd2b CB_VERSION=6.5.0
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Fri, 21 Feb 2020 23:23:08 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Fri, 21 Feb 2020 23:23:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 21 Feb 2020 23:23:08 GMT
CMD ["couchbase-server"]
# Fri, 21 Feb 2020 23:23:08 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Fri, 21 Feb 2020 23:23:08 GMT
VOLUME [/opt/couchbase/var]
```

-	Layers:
	-	`sha256:fe703b657a32e0046dce0ad2cb17172cbec8ba302edf370f5f28962bdb6216a9`  
		Last Modified: Thu, 13 Feb 2020 00:25:54 GMT  
		Size: 44.2 MB (44191726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9df1fafd224fae3ba34a68dfc401f75bf6bc0c016fe36c61661ca5c7ad729ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a645a4b887f9613f80fae43432e46423f196a9952d11bb620bef2add7c4ed4ee`  
		Last Modified: Fri, 21 Feb 2020 22:23:12 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57db7fe0b522b7a6069e769606e5ed0913a64e1e0d0030382a922ccf9449211e`  
		Last Modified: Fri, 21 Feb 2020 22:23:13 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37acf92bdab20e91916c20a5968e5cb55bcec6d8043d20d2d27ae940ae34295b`  
		Last Modified: Fri, 21 Feb 2020 23:24:20 GMT  
		Size: 5.9 MB (5853564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10cf7308a312b01ad29f3f16409e364a3b34aea3851e261329323c3781752721`  
		Last Modified: Fri, 21 Feb 2020 23:24:19 GMT  
		Size: 2.1 KB (2081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45a9b3e71d633ebcbc6710221ff737e0c62018e010599f198b986e8b5884e3e`  
		Last Modified: Fri, 21 Feb 2020 23:25:18 GMT  
		Size: 505.8 MB (505806202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33af0d5a0317b1e1e74f02478f15a311677873bce21048f8b769419ff529b9d8`  
		Last Modified: Fri, 21 Feb 2020 23:24:19 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20304ddc237219a10e926344052e99e6fd41d2607651f44bbc2d56061b6b46f7`  
		Last Modified: Fri, 21 Feb 2020 23:24:17 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d5c28589d3b2def6eb96123639d8150cdbf73f17fbcdf3b1e38d8cae058499`  
		Last Modified: Fri, 21 Feb 2020 23:24:18 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50435a6426b6a1b0b3972af671594ec5666a008e3afffc1b1b22818b2039723d`  
		Last Modified: Fri, 21 Feb 2020 23:24:18 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15a41097a0fbceab6d0bae1b81e7310b93de80b0d734d9dd56eced0fab028c0c`  
		Last Modified: Fri, 21 Feb 2020 23:24:18 GMT  
		Size: 118.1 KB (118066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4416145aaa814cce0a7e06b2c85f524f18fda317ad66a427f845d80f94ce1a2f`  
		Last Modified: Fri, 21 Feb 2020 23:24:18 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
