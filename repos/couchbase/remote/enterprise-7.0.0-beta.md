## `couchbase:enterprise-7.0.0-beta`

```console
$ docker pull couchbase@sha256:c65b3719edcc4576a926d3705e1de2f5a16c2564f11be72cde8f33c0759e3919
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `couchbase:enterprise-7.0.0-beta` - linux; amd64

```console
$ docker pull couchbase@sha256:9a13e0c08b4faa86ddd806c52c046d164686140fafecdef00c6de7210767bc67
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **616.2 MB (616172561 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91c4ba102bc002038928a18b6131545c5e071eb09579dc71d4e753ba2032ca83`
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
# Wed, 18 Nov 2020 16:57:46 GMT
ARG CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb
# Wed, 18 Nov 2020 16:57:46 GMT
ARG CB_SHA256=b345bb3f81332fe93e87966426f3b53205486fbe4902991a57566381a7ad217b
# Wed, 18 Nov 2020 16:57:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/couchbase/bin:/opt/couchbase/bin/tools:/opt/couchbase/bin/install
# Wed, 18 Nov 2020 16:57:48 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=b345bb3f81332fe93e87966426f3b53205486fbe4902991a57566381a7ad217b CB_VERSION=7.0.0-beta
RUN groupadd -g 1000 couchbase && useradd couchbase -u 1000 -g couchbase -M
# Wed, 18 Nov 2020 16:58:58 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=b345bb3f81332fe93e87966426f3b53205486fbe4902991a57566381a7ad217b CB_VERSION=7.0.0-beta
RUN export INSTALL_DONT_START_SERVER=1 &&     wget -N --no-verbose $CB_RELEASE_URL/$CB_PACKAGE &&     echo "$CB_SHA256  $CB_PACKAGE" | sha256sum -c - &&     dpkg -i ./$CB_PACKAGE && rm -f ./$CB_PACKAGE
# Wed, 18 Nov 2020 16:58:59 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=b345bb3f81332fe93e87966426f3b53205486fbe4902991a57566381a7ad217b CB_VERSION=7.0.0-beta
RUN sed -i -e '1 s/$/\/docker/' /opt/couchbase/VARIANT.txt
# Wed, 18 Nov 2020 16:59:00 GMT
COPY file:d6a307209223b2df102f46f07fd186e09fac7114db2c965bb54097d3b4d3b989 in /etc/service/couchbase-server/run 
# Wed, 18 Nov 2020 16:59:01 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=b345bb3f81332fe93e87966426f3b53205486fbe4902991a57566381a7ad217b CB_VERSION=7.0.0-beta
RUN chown -R couchbase:couchbase /etc/service
# Wed, 18 Nov 2020 16:59:01 GMT
COPY file:1302333e9e56b11ae357341056dee0080efda9457b1ce3de1a1ecb6023e760ae in /usr/local/bin/ 
# Wed, 18 Nov 2020 16:59:02 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=b345bb3f81332fe93e87966426f3b53205486fbe4902991a57566381a7ad217b CB_VERSION=7.0.0-beta
RUN ln -s dummy.sh /usr/local/bin/iptables-save &&     ln -s dummy.sh /usr/local/bin/lvdisplay &&     ln -s dummy.sh /usr/local/bin/vgdisplay &&     ln -s dummy.sh /usr/local/bin/pvdisplay
# Wed, 18 Nov 2020 16:59:03 GMT
# ARGS: CB_PACKAGE=couchbase-server-enterprise_7.0.0-beta-ubuntu20.04_amd64.deb CB_RELEASE_URL=https://packages.couchbase.com/releases/7.0.0-beta CB_SHA256=b345bb3f81332fe93e87966426f3b53205486fbe4902991a57566381a7ad217b CB_VERSION=7.0.0-beta
RUN chrpath -r '$ORIGIN/../lib' /opt/couchbase/bin/curl
# Wed, 18 Nov 2020 16:59:04 GMT
COPY file:d816a67f62bfba76d2812cefbe92252afa13f3852775c3e68599df7741e90cb7 in / 
# Wed, 18 Nov 2020 16:59:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 18 Nov 2020 16:59:08 GMT
CMD ["couchbase-server"]
# Wed, 18 Nov 2020 16:59:10 GMT
EXPOSE 11207 11210 11211 18091 18092 18093 18094 18095 18096 8091 8092 8093 8094 8095 8096
# Wed, 18 Nov 2020 16:59:12 GMT
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
	-	`sha256:8e9d012e1464eb4c6fdac3bd46b35366e9aa3a688061f34122e3f22cdb458c6c`  
		Last Modified: Wed, 18 Nov 2020 17:00:46 GMT  
		Size: 1.8 KB (1835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbab049db3ebf6b3eb28815e884c8e9b07b2b1ba30b1db9a8ff62705c889933c`  
		Last Modified: Wed, 18 Nov 2020 17:02:04 GMT  
		Size: 581.2 MB (581205296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8144f33776615d6a54feca082db40b4c1318938335284d1c191ed3af8e0e906c`  
		Last Modified: Wed, 18 Nov 2020 17:00:46 GMT  
		Size: 191.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5f6e36af6b74453240494642b5f404e0aa528480066a27234735938a00299ac`  
		Last Modified: Wed, 18 Nov 2020 17:00:46 GMT  
		Size: 452.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b8553a9de8cc88ce285320f92570f8198ad2b8eeac1162e4e83907a98e2b36`  
		Last Modified: Wed, 18 Nov 2020 17:00:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cd0fa0afe26aeb9fa7505036f9b89c8f0badcfe6c7743e7d1bc60ab5a984b34`  
		Last Modified: Wed, 18 Nov 2020 17:00:44 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df50a27063725b288c36f9e241b25cb1e6f3842a62fff9d634b87c2c3471a2e`  
		Last Modified: Wed, 18 Nov 2020 17:00:44 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c960806a1ec532c1c89c4d38c548e76a9c0f6e3b919200a9f79e0361d82d4b66`  
		Last Modified: Wed, 18 Nov 2020 17:00:44 GMT  
		Size: 125.9 KB (125893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d545bfb73af04a8ef58ab82314447d78bc9728747325992c878ba0cca9bb86`  
		Last Modified: Wed, 18 Nov 2020 17:00:44 GMT  
		Size: 857.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
