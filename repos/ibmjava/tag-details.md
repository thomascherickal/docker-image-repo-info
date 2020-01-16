<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `ibmjava`

-	[`ibmjava:8`](#ibmjava8)
-	[`ibmjava:8-jre`](#ibmjava8-jre)
-	[`ibmjava:8-jre-alpine`](#ibmjava8-jre-alpine)
-	[`ibmjava:8-sdk`](#ibmjava8-sdk)
-	[`ibmjava:8-sdk-alpine`](#ibmjava8-sdk-alpine)
-	[`ibmjava:8-sfj`](#ibmjava8-sfj)
-	[`ibmjava:8-sfj-alpine`](#ibmjava8-sfj-alpine)
-	[`ibmjava:jre`](#ibmjavajre)
-	[`ibmjava:jre-alpine`](#ibmjavajre-alpine)
-	[`ibmjava:latest`](#ibmjavalatest)
-	[`ibmjava:sdk`](#ibmjavasdk)
-	[`ibmjava:sdk-alpine`](#ibmjavasdk-alpine)
-	[`ibmjava:sfj`](#ibmjavasfj)
-	[`ibmjava:sfj-alpine`](#ibmjavasfj-alpine)

## `ibmjava:8`

```console
$ docker pull ibmjava@sha256:8632798b1e75ac2023a6b444689516cf2b842d52cdbbceb2a55265412ea8aa35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8` - linux; amd64

```console
$ docker pull ibmjava@sha256:534f96dcd6dd31abb7e4ef8642446db018310ae282bf400265b3e5320ee84ac6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.9 MB (159902184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f724821d61dbab3904487d424d8e2ade96f509f56cc7df2279982c6019fc53b3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 03:27:18 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 03:27:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:27:26 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 03:28:09 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='31a6f7e851749343cb4fe3956202bdde0beabff901ba926e78cdf013e6d7e725';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='35d0aa5e54b8d68873a2b5de27e834ff4801dcaf598e180b820366f902cef345';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e10ce4e0ba88febefeffef246d59a746c6b9cbe3a3259c792bcf5af807304332';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='bfdb5e450cf4dc9d6f322e8969bb9e7c75d371e38ebf325c635b91ff55eb3ffb';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='3956e363357c68e60c5df1e98a51f75f2e680c237320dea59a02b38e5541ce23';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 03:28:10 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5b7faea59f26f78539055a47552f83601485924313dee5f2d3905977a43aac`  
		Last Modified: Thu, 16 Jan 2020 03:30:20 GMT  
		Size: 3.0 MB (2965136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fed68b301d333ece91cd1852e1757b3b1e70a7db7896318a6dfa3736ff5a3e`  
		Last Modified: Thu, 16 Jan 2020 03:30:32 GMT  
		Size: 130.2 MB (130210480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8` - linux; 386

```console
$ docker pull ibmjava@sha256:b55ac8e9ae572334a390204a9a78576fe1c6247aabe4d010fcc9cbbdba6fcace
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.8 MB (148826484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ecba5a21ae87b618ad2a7d5b0d9d9ff261e6e8e8758426e8b3c9b39e0730622`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:38:58 GMT
ADD file:2c41d212af13e7724c6bec90702f30ad85119de23c2ac29494a848e31c568f0f in / 
# Thu, 16 Jan 2020 00:38:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:38:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:39:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:39:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 00:55:58 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 00:56:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:56:07 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 00:56:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='31a6f7e851749343cb4fe3956202bdde0beabff901ba926e78cdf013e6d7e725';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='35d0aa5e54b8d68873a2b5de27e834ff4801dcaf598e180b820366f902cef345';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e10ce4e0ba88febefeffef246d59a746c6b9cbe3a3259c792bcf5af807304332';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='bfdb5e450cf4dc9d6f322e8969bb9e7c75d371e38ebf325c635b91ff55eb3ffb';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='3956e363357c68e60c5df1e98a51f75f2e680c237320dea59a02b38e5541ce23';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 00:56:50 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:0486f132427cc5680d6c6a730e5b518a472f5d0aed43b4c033d3ca9d7f297f21`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 27.1 MB (27122980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884577b2a5cf120bc140e290f06a80bb60802cdc3e0818d2bdb08b724a5a14ef`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 34.6 KB (34620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec417e00c26f6fb4ebd128ca352ab1d4f89b8d9bd06fecdf9a5a64e56c6140b`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c45ceba8ba99dbaa734783259d2a1d46c1ccccbae9bea76e70bbf7629016f5`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8938cf79804632fc6f2701a40497a749ebb1e90d30fec2defad2a8ea1ed872`  
		Last Modified: Thu, 16 Jan 2020 00:58:47 GMT  
		Size: 3.0 MB (2992068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23dcccd16c67a87b392bdc0f10e158d212ca6e0e40a3c23d7b695cd8e60ff23`  
		Last Modified: Thu, 16 Jan 2020 00:58:59 GMT  
		Size: 118.7 MB (118675804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:17220ba5d73526dfab8fd9ac4a25b7bc4c503e98f8a05a854eaea0c26bb9e849
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176650569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cba4d0a13eaabd29ca4fe3effacb4896b6a96f1eb757e915bb63a07155b0c18a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:16:57 GMT
ADD file:9a1a27f07b5eac878569b1a3279d14f876400a0bbb293be818f5554662ac82e9 in / 
# Thu, 16 Jan 2020 01:17:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:17:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:17:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:17:19 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:36:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 01:37:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:37:18 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 01:38:22 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='31a6f7e851749343cb4fe3956202bdde0beabff901ba926e78cdf013e6d7e725';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='35d0aa5e54b8d68873a2b5de27e834ff4801dcaf598e180b820366f902cef345';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e10ce4e0ba88febefeffef246d59a746c6b9cbe3a3259c792bcf5af807304332';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='bfdb5e450cf4dc9d6f322e8969bb9e7c75d371e38ebf325c635b91ff55eb3ffb';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='3956e363357c68e60c5df1e98a51f75f2e680c237320dea59a02b38e5541ce23';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 01:38:25 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5592aacf4ac7489bb730c3e5b1799876d68000b7bbf6e9377ca30e16bff059be`  
		Last Modified: Mon, 13 Jan 2020 15:33:24 GMT  
		Size: 30.4 MB (30400610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f7f270f33afb11e2590bebf54c54fcb052048417bc01b24e357117d730d26a`  
		Last Modified: Thu, 16 Jan 2020 01:19:43 GMT  
		Size: 35.2 KB (35217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242585cde72a9805b281397c8fe3b84a8260c6523a4c290da82e6209845c3690`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509fc799f2e0e3149ea8c75fb5b36528e147c5e7123e226d9da46be9c3c79f36`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a14c8ba333672ab64ed6968f103d9a6647e0d49e0789bce7d2a0ebe424b3f5`  
		Last Modified: Thu, 16 Jan 2020 01:41:06 GMT  
		Size: 3.1 MB (3093271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebc985f96c0a80fddf0aa8dc2dc8e4ea2b6e8c213780a630d4e05f25a4a6f28`  
		Last Modified: Thu, 16 Jan 2020 01:41:23 GMT  
		Size: 143.1 MB (143120427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8` - linux; s390x

```console
$ docker pull ibmjava@sha256:055430c5163aaeaf101eeff35333202248b9b16790e2ed77d0ec9d39273bfb55
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155583788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3869571e8106ebd89dae543a34aa9b11682ef9e97849d54484afb0fc0b2a6129`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:45:22 GMT
ADD file:4f49a0df2ce5765780345889c57bfaeff1b44de88f7aa876b30ae4f4aa4b1f54 in / 
# Thu, 16 Jan 2020 00:45:23 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:45:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:45:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:45:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:11:09 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 01:11:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:11:15 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 01:11:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='31a6f7e851749343cb4fe3956202bdde0beabff901ba926e78cdf013e6d7e725';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='35d0aa5e54b8d68873a2b5de27e834ff4801dcaf598e180b820366f902cef345';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e10ce4e0ba88febefeffef246d59a746c6b9cbe3a3259c792bcf5af807304332';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='bfdb5e450cf4dc9d6f322e8969bb9e7c75d371e38ebf325c635b91ff55eb3ffb';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='3956e363357c68e60c5df1e98a51f75f2e680c237320dea59a02b38e5541ce23';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 01:11:54 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5e33acada67b43fd81daf3ea8c5b66f480d30d8e6b52e8e3c803d4fe94166024`  
		Last Modified: Mon, 13 Jan 2020 15:34:25 GMT  
		Size: 25.4 MB (25365173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be29508430b95a934d4b70805c50ebe81d716b5aa5b1a3e7d7e674f8c74325dd`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 36.2 KB (36179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed40edcc110aecf91ae3ae074beb10680df57608ad36a93af18548b9c7a49bf2`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f85c1c8cfa969830d1386d6be3d6c989dedcc0a2c65226d4c760a9ec64499b7`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56619e028711aff32431a988d23695bbfd65e0d5f180d8c60579079a24fcedfa`  
		Last Modified: Thu, 16 Jan 2020 01:13:32 GMT  
		Size: 2.7 MB (2678579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d1d179e2201862ab782a8b7943234954684ea1750a3302221d2ee8e7c2360b`  
		Last Modified: Thu, 16 Jan 2020 01:13:42 GMT  
		Size: 127.5 MB (127502848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-jre`

```console
$ docker pull ibmjava@sha256:8632798b1e75ac2023a6b444689516cf2b842d52cdbbceb2a55265412ea8aa35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-jre` - linux; amd64

```console
$ docker pull ibmjava@sha256:534f96dcd6dd31abb7e4ef8642446db018310ae282bf400265b3e5320ee84ac6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.9 MB (159902184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f724821d61dbab3904487d424d8e2ade96f509f56cc7df2279982c6019fc53b3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 03:27:18 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 03:27:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:27:26 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 03:28:09 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='31a6f7e851749343cb4fe3956202bdde0beabff901ba926e78cdf013e6d7e725';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='35d0aa5e54b8d68873a2b5de27e834ff4801dcaf598e180b820366f902cef345';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e10ce4e0ba88febefeffef246d59a746c6b9cbe3a3259c792bcf5af807304332';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='bfdb5e450cf4dc9d6f322e8969bb9e7c75d371e38ebf325c635b91ff55eb3ffb';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='3956e363357c68e60c5df1e98a51f75f2e680c237320dea59a02b38e5541ce23';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 03:28:10 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5b7faea59f26f78539055a47552f83601485924313dee5f2d3905977a43aac`  
		Last Modified: Thu, 16 Jan 2020 03:30:20 GMT  
		Size: 3.0 MB (2965136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fed68b301d333ece91cd1852e1757b3b1e70a7db7896318a6dfa3736ff5a3e`  
		Last Modified: Thu, 16 Jan 2020 03:30:32 GMT  
		Size: 130.2 MB (130210480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-jre` - linux; 386

```console
$ docker pull ibmjava@sha256:b55ac8e9ae572334a390204a9a78576fe1c6247aabe4d010fcc9cbbdba6fcace
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.8 MB (148826484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ecba5a21ae87b618ad2a7d5b0d9d9ff261e6e8e8758426e8b3c9b39e0730622`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:38:58 GMT
ADD file:2c41d212af13e7724c6bec90702f30ad85119de23c2ac29494a848e31c568f0f in / 
# Thu, 16 Jan 2020 00:38:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:38:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:39:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:39:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 00:55:58 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 00:56:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:56:07 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 00:56:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='31a6f7e851749343cb4fe3956202bdde0beabff901ba926e78cdf013e6d7e725';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='35d0aa5e54b8d68873a2b5de27e834ff4801dcaf598e180b820366f902cef345';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e10ce4e0ba88febefeffef246d59a746c6b9cbe3a3259c792bcf5af807304332';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='bfdb5e450cf4dc9d6f322e8969bb9e7c75d371e38ebf325c635b91ff55eb3ffb';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='3956e363357c68e60c5df1e98a51f75f2e680c237320dea59a02b38e5541ce23';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 00:56:50 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:0486f132427cc5680d6c6a730e5b518a472f5d0aed43b4c033d3ca9d7f297f21`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 27.1 MB (27122980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884577b2a5cf120bc140e290f06a80bb60802cdc3e0818d2bdb08b724a5a14ef`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 34.6 KB (34620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec417e00c26f6fb4ebd128ca352ab1d4f89b8d9bd06fecdf9a5a64e56c6140b`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c45ceba8ba99dbaa734783259d2a1d46c1ccccbae9bea76e70bbf7629016f5`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8938cf79804632fc6f2701a40497a749ebb1e90d30fec2defad2a8ea1ed872`  
		Last Modified: Thu, 16 Jan 2020 00:58:47 GMT  
		Size: 3.0 MB (2992068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23dcccd16c67a87b392bdc0f10e158d212ca6e0e40a3c23d7b695cd8e60ff23`  
		Last Modified: Thu, 16 Jan 2020 00:58:59 GMT  
		Size: 118.7 MB (118675804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-jre` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:17220ba5d73526dfab8fd9ac4a25b7bc4c503e98f8a05a854eaea0c26bb9e849
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176650569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cba4d0a13eaabd29ca4fe3effacb4896b6a96f1eb757e915bb63a07155b0c18a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:16:57 GMT
ADD file:9a1a27f07b5eac878569b1a3279d14f876400a0bbb293be818f5554662ac82e9 in / 
# Thu, 16 Jan 2020 01:17:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:17:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:17:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:17:19 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:36:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 01:37:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:37:18 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 01:38:22 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='31a6f7e851749343cb4fe3956202bdde0beabff901ba926e78cdf013e6d7e725';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='35d0aa5e54b8d68873a2b5de27e834ff4801dcaf598e180b820366f902cef345';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e10ce4e0ba88febefeffef246d59a746c6b9cbe3a3259c792bcf5af807304332';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='bfdb5e450cf4dc9d6f322e8969bb9e7c75d371e38ebf325c635b91ff55eb3ffb';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='3956e363357c68e60c5df1e98a51f75f2e680c237320dea59a02b38e5541ce23';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 01:38:25 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5592aacf4ac7489bb730c3e5b1799876d68000b7bbf6e9377ca30e16bff059be`  
		Last Modified: Mon, 13 Jan 2020 15:33:24 GMT  
		Size: 30.4 MB (30400610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f7f270f33afb11e2590bebf54c54fcb052048417bc01b24e357117d730d26a`  
		Last Modified: Thu, 16 Jan 2020 01:19:43 GMT  
		Size: 35.2 KB (35217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242585cde72a9805b281397c8fe3b84a8260c6523a4c290da82e6209845c3690`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509fc799f2e0e3149ea8c75fb5b36528e147c5e7123e226d9da46be9c3c79f36`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a14c8ba333672ab64ed6968f103d9a6647e0d49e0789bce7d2a0ebe424b3f5`  
		Last Modified: Thu, 16 Jan 2020 01:41:06 GMT  
		Size: 3.1 MB (3093271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebc985f96c0a80fddf0aa8dc2dc8e4ea2b6e8c213780a630d4e05f25a4a6f28`  
		Last Modified: Thu, 16 Jan 2020 01:41:23 GMT  
		Size: 143.1 MB (143120427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-jre` - linux; s390x

```console
$ docker pull ibmjava@sha256:055430c5163aaeaf101eeff35333202248b9b16790e2ed77d0ec9d39273bfb55
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155583788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3869571e8106ebd89dae543a34aa9b11682ef9e97849d54484afb0fc0b2a6129`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:45:22 GMT
ADD file:4f49a0df2ce5765780345889c57bfaeff1b44de88f7aa876b30ae4f4aa4b1f54 in / 
# Thu, 16 Jan 2020 00:45:23 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:45:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:45:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:45:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:11:09 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 01:11:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:11:15 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 01:11:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='31a6f7e851749343cb4fe3956202bdde0beabff901ba926e78cdf013e6d7e725';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='35d0aa5e54b8d68873a2b5de27e834ff4801dcaf598e180b820366f902cef345';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e10ce4e0ba88febefeffef246d59a746c6b9cbe3a3259c792bcf5af807304332';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='bfdb5e450cf4dc9d6f322e8969bb9e7c75d371e38ebf325c635b91ff55eb3ffb';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='3956e363357c68e60c5df1e98a51f75f2e680c237320dea59a02b38e5541ce23';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 01:11:54 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5e33acada67b43fd81daf3ea8c5b66f480d30d8e6b52e8e3c803d4fe94166024`  
		Last Modified: Mon, 13 Jan 2020 15:34:25 GMT  
		Size: 25.4 MB (25365173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be29508430b95a934d4b70805c50ebe81d716b5aa5b1a3e7d7e674f8c74325dd`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 36.2 KB (36179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed40edcc110aecf91ae3ae074beb10680df57608ad36a93af18548b9c7a49bf2`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f85c1c8cfa969830d1386d6be3d6c989dedcc0a2c65226d4c760a9ec64499b7`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56619e028711aff32431a988d23695bbfd65e0d5f180d8c60579079a24fcedfa`  
		Last Modified: Thu, 16 Jan 2020 01:13:32 GMT  
		Size: 2.7 MB (2678579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d1d179e2201862ab782a8b7943234954684ea1750a3302221d2ee8e7c2360b`  
		Last Modified: Thu, 16 Jan 2020 01:13:42 GMT  
		Size: 127.5 MB (127502848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-jre-alpine`

```console
$ docker pull ibmjava@sha256:2e7f4d0cccf8c3acfe20ae86daf984a8f7f6d13e32622cbff36dbb03d441349a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `ibmjava:8-jre-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:448e176743d26d21965f9ac27233c9e7467240855f4d2cef95569239ddf5ab12
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138524117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56d0d02bb75b7565fae1266b537cf055a0785626d00f2db2a815ee9ac771db2f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 17:39:11 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Mon, 21 Oct 2019 17:39:11 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Mon, 21 Oct 2019 17:39:30 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Thu, 28 Nov 2019 20:21:10 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 28 Nov 2019 20:21:50 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='31a6f7e851749343cb4fe3956202bdde0beabff901ba926e78cdf013e6d7e725';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='35d0aa5e54b8d68873a2b5de27e834ff4801dcaf598e180b820366f902cef345';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e10ce4e0ba88febefeffef246d59a746c6b9cbe3a3259c792bcf5af807304332';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='bfdb5e450cf4dc9d6f322e8969bb9e7c75d371e38ebf325c635b91ff55eb3ffb';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='3956e363357c68e60c5df1e98a51f75f2e680c237320dea59a02b38e5541ce23';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Thu, 28 Nov 2019 20:21:50 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd10b3e3ffcf891c3573e370dd214e57c0fc41b96cd920b99f8cb3f118cbbc8`  
		Last Modified: Mon, 21 Oct 2019 17:42:11 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465dff0793d236fe777baf5eb7dd6453017983c9d74ae8aae40ee2a11ba6c369`  
		Last Modified: Mon, 21 Oct 2019 17:42:12 GMT  
		Size: 5.6 MB (5565596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e617b8a4160f048792788dc0a5e4566852cd4c999c23f99fedd388203e1c8b`  
		Last Modified: Thu, 28 Nov 2019 20:25:41 GMT  
		Size: 130.2 MB (130170842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-sdk`

```console
$ docker pull ibmjava@sha256:9b27a9d9c33e484f25bd4ff71ca5e19c4ebc1bc2b9606392ac02fb7bf279ed9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-sdk` - linux; amd64

```console
$ docker pull ibmjava@sha256:2eb69e6b419e6ccb51201bf7913bd7a70c6cb8fe29458f424a75ea5467a2de36
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.1 MB (197062481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6916b880c33ec4b03b8172bd6056e1fb5204a70140334ebefbe95236e041dec0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 03:27:18 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 03:27:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:27:26 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 03:29:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='4c3b62dc988223239d0049e03c40444524356e3cdf805972e1a35d127d00c1c9';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='8618f9ed7bd5575f17ea9e63d8c37f2afa283bf6c9c240bd6f7eba18642c1227';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='18c2eccf99225e6e7643141d8da4110cacc39f2fa00149fc26341d2272cc0102';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='095f80d219f95158e1b734d1632b40dc1aaa457fd04e23e04e6e9667adc8bf48';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='97e45a2fffa1ec8c57da614313cbb32d430210ae18e22c7022cd18204ea5ec96';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 03:29:58 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5b7faea59f26f78539055a47552f83601485924313dee5f2d3905977a43aac`  
		Last Modified: Thu, 16 Jan 2020 03:30:20 GMT  
		Size: 3.0 MB (2965136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821c49691759d482d6d0ba4f40279447943769f0e477d9b4f2e2e65af884bb2e`  
		Last Modified: Thu, 16 Jan 2020 03:31:08 GMT  
		Size: 167.4 MB (167370777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; 386

```console
$ docker pull ibmjava@sha256:fdfbcbababd489a0feba701d2f75d92a4d50a441f4cf2d546c3d16e1377828a4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.9 MB (185874249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df8fe399784d565a9f6b8894520c0f5f8f9c2bf4e3951a5e3b587c5a4b67133f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:38:58 GMT
ADD file:2c41d212af13e7724c6bec90702f30ad85119de23c2ac29494a848e31c568f0f in / 
# Thu, 16 Jan 2020 00:38:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:38:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:39:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:39:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 00:55:58 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 00:56:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:56:07 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 00:58:29 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='4c3b62dc988223239d0049e03c40444524356e3cdf805972e1a35d127d00c1c9';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='8618f9ed7bd5575f17ea9e63d8c37f2afa283bf6c9c240bd6f7eba18642c1227';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='18c2eccf99225e6e7643141d8da4110cacc39f2fa00149fc26341d2272cc0102';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='095f80d219f95158e1b734d1632b40dc1aaa457fd04e23e04e6e9667adc8bf48';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='97e45a2fffa1ec8c57da614313cbb32d430210ae18e22c7022cd18204ea5ec96';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 00:58:30 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:0486f132427cc5680d6c6a730e5b518a472f5d0aed43b4c033d3ca9d7f297f21`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 27.1 MB (27122980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884577b2a5cf120bc140e290f06a80bb60802cdc3e0818d2bdb08b724a5a14ef`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 34.6 KB (34620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec417e00c26f6fb4ebd128ca352ab1d4f89b8d9bd06fecdf9a5a64e56c6140b`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c45ceba8ba99dbaa734783259d2a1d46c1ccccbae9bea76e70bbf7629016f5`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8938cf79804632fc6f2701a40497a749ebb1e90d30fec2defad2a8ea1ed872`  
		Last Modified: Thu, 16 Jan 2020 00:58:47 GMT  
		Size: 3.0 MB (2992068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426f3d330e3eea8713e33b004242816bcf884f9eb046e03ca4f66289441458a7`  
		Last Modified: Thu, 16 Jan 2020 00:59:50 GMT  
		Size: 155.7 MB (155723569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:1f35a2bccb16bf654639e48f32729bc6f940c76074d3151a2908c4db5342722f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.9 MB (213928209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a6d6449090b49333e2e3f800f4e19b7456de1e90359caf5b5a0d20b600d1bef`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:16:57 GMT
ADD file:9a1a27f07b5eac878569b1a3279d14f876400a0bbb293be818f5554662ac82e9 in / 
# Thu, 16 Jan 2020 01:17:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:17:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:17:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:17:19 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:36:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 01:37:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:37:18 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 01:40:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='4c3b62dc988223239d0049e03c40444524356e3cdf805972e1a35d127d00c1c9';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='8618f9ed7bd5575f17ea9e63d8c37f2afa283bf6c9c240bd6f7eba18642c1227';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='18c2eccf99225e6e7643141d8da4110cacc39f2fa00149fc26341d2272cc0102';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='095f80d219f95158e1b734d1632b40dc1aaa457fd04e23e04e6e9667adc8bf48';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='97e45a2fffa1ec8c57da614313cbb32d430210ae18e22c7022cd18204ea5ec96';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 01:40:48 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5592aacf4ac7489bb730c3e5b1799876d68000b7bbf6e9377ca30e16bff059be`  
		Last Modified: Mon, 13 Jan 2020 15:33:24 GMT  
		Size: 30.4 MB (30400610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f7f270f33afb11e2590bebf54c54fcb052048417bc01b24e357117d730d26a`  
		Last Modified: Thu, 16 Jan 2020 01:19:43 GMT  
		Size: 35.2 KB (35217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242585cde72a9805b281397c8fe3b84a8260c6523a4c290da82e6209845c3690`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509fc799f2e0e3149ea8c75fb5b36528e147c5e7123e226d9da46be9c3c79f36`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a14c8ba333672ab64ed6968f103d9a6647e0d49e0789bce7d2a0ebe424b3f5`  
		Last Modified: Thu, 16 Jan 2020 01:41:06 GMT  
		Size: 3.1 MB (3093271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e610c730b6954c1f9636195c0e065064a88c1f0a365feacb864a7b1fdff230`  
		Last Modified: Thu, 16 Jan 2020 01:42:47 GMT  
		Size: 180.4 MB (180398067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; s390x

```console
$ docker pull ibmjava@sha256:bc4984ac270a50360519efb0e514297ccdca2ed333624a2d4f238d8b6a0844ff
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.8 MB (185829502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1f7dad284aac0e12062652652f3a10ddb45f397a1306e70307dd503bcc85e72`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:45:22 GMT
ADD file:4f49a0df2ce5765780345889c57bfaeff1b44de88f7aa876b30ae4f4aa4b1f54 in / 
# Thu, 16 Jan 2020 00:45:23 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:45:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:45:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:45:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:11:09 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 01:11:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:11:15 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 01:13:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='4c3b62dc988223239d0049e03c40444524356e3cdf805972e1a35d127d00c1c9';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='8618f9ed7bd5575f17ea9e63d8c37f2afa283bf6c9c240bd6f7eba18642c1227';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='18c2eccf99225e6e7643141d8da4110cacc39f2fa00149fc26341d2272cc0102';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='095f80d219f95158e1b734d1632b40dc1aaa457fd04e23e04e6e9667adc8bf48';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='97e45a2fffa1ec8c57da614313cbb32d430210ae18e22c7022cd18204ea5ec96';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 01:13:23 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5e33acada67b43fd81daf3ea8c5b66f480d30d8e6b52e8e3c803d4fe94166024`  
		Last Modified: Mon, 13 Jan 2020 15:34:25 GMT  
		Size: 25.4 MB (25365173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be29508430b95a934d4b70805c50ebe81d716b5aa5b1a3e7d7e674f8c74325dd`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 36.2 KB (36179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed40edcc110aecf91ae3ae074beb10680df57608ad36a93af18548b9c7a49bf2`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f85c1c8cfa969830d1386d6be3d6c989dedcc0a2c65226d4c760a9ec64499b7`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56619e028711aff32431a988d23695bbfd65e0d5f180d8c60579079a24fcedfa`  
		Last Modified: Thu, 16 Jan 2020 01:13:32 GMT  
		Size: 2.7 MB (2678579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e0d8fc0c0bc62dab86f7c970fd715f47f4969931df1563d7840df76a9b3e15`  
		Last Modified: Thu, 16 Jan 2020 01:14:11 GMT  
		Size: 157.7 MB (157748562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-sdk-alpine`

```console
$ docker pull ibmjava@sha256:90199ebb409616ca8b538efea2ad290b5835876649ac23fbb3e674694498edb6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `ibmjava:8-sdk-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:c7edb4c364882cfef4ac405cbb65e6fd936cfde5ad2b554ac7c6a30dca41d867
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.7 MB (175679272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:675ab2389e990d2b76715850754687213245217e7720c90677bf731f2e852aaf`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 17:39:11 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Mon, 21 Oct 2019 17:39:11 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Mon, 21 Oct 2019 17:39:30 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Thu, 28 Nov 2019 20:21:10 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 28 Nov 2019 20:24:59 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='4c3b62dc988223239d0049e03c40444524356e3cdf805972e1a35d127d00c1c9';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='8618f9ed7bd5575f17ea9e63d8c37f2afa283bf6c9c240bd6f7eba18642c1227';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='18c2eccf99225e6e7643141d8da4110cacc39f2fa00149fc26341d2272cc0102';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='095f80d219f95158e1b734d1632b40dc1aaa457fd04e23e04e6e9667adc8bf48';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='97e45a2fffa1ec8c57da614313cbb32d430210ae18e22c7022cd18204ea5ec96';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Thu, 28 Nov 2019 20:24:59 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd10b3e3ffcf891c3573e370dd214e57c0fc41b96cd920b99f8cb3f118cbbc8`  
		Last Modified: Mon, 21 Oct 2019 17:42:11 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465dff0793d236fe777baf5eb7dd6453017983c9d74ae8aae40ee2a11ba6c369`  
		Last Modified: Mon, 21 Oct 2019 17:42:12 GMT  
		Size: 5.6 MB (5565596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ea3903d89773e915cc11ad7083d8d6c04c8ed4b3623a0f628a1721a0f51831`  
		Last Modified: Thu, 28 Nov 2019 20:26:46 GMT  
		Size: 167.3 MB (167325997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-sfj`

```console
$ docker pull ibmjava@sha256:287008706919354c0fc9b4f93edfdf7fedcd74e87641405da2acc0974a08e52e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-sfj` - linux; amd64

```console
$ docker pull ibmjava@sha256:8767aebf1906a826a198dc5db305747c7fa2e449fdf1e73800a28a2ebf5baad2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93210577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3564b44cc8e2dc75197cc0e9ddcdb99699b0b1aa1d508a3a1dc8569e7b86e75`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 03:27:18 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 03:27:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:27:26 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 03:28:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='822b2bd8286c2ec4a7dd7f84386be3ccf43f0f1c3e259c4ed96aac3210d3e11a';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='4147cb108ea191199ca86d298692d87381f354ce0b15e22c2bcadc0f49a1af4a';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='fbe53ee7151f624b6119106373115d319554cc1760b32dee6c37113157d1c773';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='cc0b10e220eca7e6c76a2d461018055e2e41e0f532d8ddf08c7dd7eb06770f14';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='81962223b3e439e2d9a8e38b51ffc5f80f18884216fd41647192baebf4829708';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 03:28:58 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5b7faea59f26f78539055a47552f83601485924313dee5f2d3905977a43aac`  
		Last Modified: Thu, 16 Jan 2020 03:30:20 GMT  
		Size: 3.0 MB (2965136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff65401a9d7a35b6c3ad2220d1593d6406450066542fd5b3683fb96b84ffa357`  
		Last Modified: Thu, 16 Jan 2020 03:30:50 GMT  
		Size: 63.5 MB (63518873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; 386

```console
$ docker pull ibmjava@sha256:9b7f8545ce9c2e84cb1e274a853546f7e7788310df00a9a63150f55ca64a1123
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93095310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92e652d0abed34825e3a6ebf618d0b850870fa1fb76162bef773b3de3d778bd0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:38:58 GMT
ADD file:2c41d212af13e7724c6bec90702f30ad85119de23c2ac29494a848e31c568f0f in / 
# Thu, 16 Jan 2020 00:38:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:38:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:39:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:39:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 00:55:58 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 00:56:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:56:07 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 00:57:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='822b2bd8286c2ec4a7dd7f84386be3ccf43f0f1c3e259c4ed96aac3210d3e11a';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='4147cb108ea191199ca86d298692d87381f354ce0b15e22c2bcadc0f49a1af4a';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='fbe53ee7151f624b6119106373115d319554cc1760b32dee6c37113157d1c773';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='cc0b10e220eca7e6c76a2d461018055e2e41e0f532d8ddf08c7dd7eb06770f14';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='81962223b3e439e2d9a8e38b51ffc5f80f18884216fd41647192baebf4829708';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 00:57:34 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:0486f132427cc5680d6c6a730e5b518a472f5d0aed43b4c033d3ca9d7f297f21`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 27.1 MB (27122980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884577b2a5cf120bc140e290f06a80bb60802cdc3e0818d2bdb08b724a5a14ef`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 34.6 KB (34620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec417e00c26f6fb4ebd128ca352ab1d4f89b8d9bd06fecdf9a5a64e56c6140b`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c45ceba8ba99dbaa734783259d2a1d46c1ccccbae9bea76e70bbf7629016f5`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8938cf79804632fc6f2701a40497a749ebb1e90d30fec2defad2a8ea1ed872`  
		Last Modified: Thu, 16 Jan 2020 00:58:47 GMT  
		Size: 3.0 MB (2992068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1ce2aa2cc3d5e869c33a184a1345a9cd9084f7b9e6a0d2ac4075e06c1847f6`  
		Last Modified: Thu, 16 Jan 2020 00:59:14 GMT  
		Size: 62.9 MB (62944630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:f973cc82219c07335a2b02a465b31ce90e03dcdc2f1315e1049eb248e1dab406
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.6 MB (101639936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c61b6e68f1c1f6f7c31db6fda5112d80a2d09b823ef62fc4fce3e14cd56c705`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:16:57 GMT
ADD file:9a1a27f07b5eac878569b1a3279d14f876400a0bbb293be818f5554662ac82e9 in / 
# Thu, 16 Jan 2020 01:17:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:17:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:17:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:17:19 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:36:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 01:37:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:37:18 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 01:39:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='822b2bd8286c2ec4a7dd7f84386be3ccf43f0f1c3e259c4ed96aac3210d3e11a';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='4147cb108ea191199ca86d298692d87381f354ce0b15e22c2bcadc0f49a1af4a';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='fbe53ee7151f624b6119106373115d319554cc1760b32dee6c37113157d1c773';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='cc0b10e220eca7e6c76a2d461018055e2e41e0f532d8ddf08c7dd7eb06770f14';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='81962223b3e439e2d9a8e38b51ffc5f80f18884216fd41647192baebf4829708';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 01:39:19 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5592aacf4ac7489bb730c3e5b1799876d68000b7bbf6e9377ca30e16bff059be`  
		Last Modified: Mon, 13 Jan 2020 15:33:24 GMT  
		Size: 30.4 MB (30400610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f7f270f33afb11e2590bebf54c54fcb052048417bc01b24e357117d730d26a`  
		Last Modified: Thu, 16 Jan 2020 01:19:43 GMT  
		Size: 35.2 KB (35217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242585cde72a9805b281397c8fe3b84a8260c6523a4c290da82e6209845c3690`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509fc799f2e0e3149ea8c75fb5b36528e147c5e7123e226d9da46be9c3c79f36`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a14c8ba333672ab64ed6968f103d9a6647e0d49e0789bce7d2a0ebe424b3f5`  
		Last Modified: Thu, 16 Jan 2020 01:41:06 GMT  
		Size: 3.1 MB (3093271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227a44da282b869228b869e8a9c2b5f3a83403eb47d9219a37712d92e5d51d2c`  
		Last Modified: Thu, 16 Jan 2020 01:41:49 GMT  
		Size: 68.1 MB (68109794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; s390x

```console
$ docker pull ibmjava@sha256:fc47a4bd11377cfa3debbd1939cbf28481ae9a067ebc06200abccdb4a0c508cb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.8 MB (92776886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c579628c5b6fb6357794b06aff9f90319869f8b90426c1d80c88613169d27615`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:45:22 GMT
ADD file:4f49a0df2ce5765780345889c57bfaeff1b44de88f7aa876b30ae4f4aa4b1f54 in / 
# Thu, 16 Jan 2020 00:45:23 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:45:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:45:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:45:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:11:09 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 01:11:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:11:15 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 01:12:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='822b2bd8286c2ec4a7dd7f84386be3ccf43f0f1c3e259c4ed96aac3210d3e11a';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='4147cb108ea191199ca86d298692d87381f354ce0b15e22c2bcadc0f49a1af4a';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='fbe53ee7151f624b6119106373115d319554cc1760b32dee6c37113157d1c773';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='cc0b10e220eca7e6c76a2d461018055e2e41e0f532d8ddf08c7dd7eb06770f14';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='81962223b3e439e2d9a8e38b51ffc5f80f18884216fd41647192baebf4829708';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 01:12:33 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5e33acada67b43fd81daf3ea8c5b66f480d30d8e6b52e8e3c803d4fe94166024`  
		Last Modified: Mon, 13 Jan 2020 15:34:25 GMT  
		Size: 25.4 MB (25365173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be29508430b95a934d4b70805c50ebe81d716b5aa5b1a3e7d7e674f8c74325dd`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 36.2 KB (36179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed40edcc110aecf91ae3ae074beb10680df57608ad36a93af18548b9c7a49bf2`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f85c1c8cfa969830d1386d6be3d6c989dedcc0a2c65226d4c760a9ec64499b7`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56619e028711aff32431a988d23695bbfd65e0d5f180d8c60579079a24fcedfa`  
		Last Modified: Thu, 16 Jan 2020 01:13:32 GMT  
		Size: 2.7 MB (2678579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0bb0ee417b74a1fdc0d4cbb7d3f8eeab02bd9d9366220e23e4e1139c319c32`  
		Last Modified: Thu, 16 Jan 2020 01:13:55 GMT  
		Size: 64.7 MB (64695946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-sfj-alpine`

```console
$ docker pull ibmjava@sha256:2f266d2e5e9c15d7ad0a572e87109d8d644ffc05827c50b3b998e0bc5e8cf836
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `ibmjava:8-sfj-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:f019479be9bc7942a52a9b72a2a5fadf2d4a770ae875b42e44c0c7d40798ce91
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71884432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:793e22b65549745e55f78b6a266575c26aba2ef71b71e84ac11342257d0dd3c0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 17:39:11 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Mon, 21 Oct 2019 17:39:11 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Mon, 21 Oct 2019 17:39:30 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Thu, 28 Nov 2019 20:21:10 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 28 Nov 2019 20:23:03 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='822b2bd8286c2ec4a7dd7f84386be3ccf43f0f1c3e259c4ed96aac3210d3e11a';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='4147cb108ea191199ca86d298692d87381f354ce0b15e22c2bcadc0f49a1af4a';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='fbe53ee7151f624b6119106373115d319554cc1760b32dee6c37113157d1c773';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='cc0b10e220eca7e6c76a2d461018055e2e41e0f532d8ddf08c7dd7eb06770f14';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='81962223b3e439e2d9a8e38b51ffc5f80f18884216fd41647192baebf4829708';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Thu, 28 Nov 2019 20:23:03 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd10b3e3ffcf891c3573e370dd214e57c0fc41b96cd920b99f8cb3f118cbbc8`  
		Last Modified: Mon, 21 Oct 2019 17:42:11 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465dff0793d236fe777baf5eb7dd6453017983c9d74ae8aae40ee2a11ba6c369`  
		Last Modified: Mon, 21 Oct 2019 17:42:12 GMT  
		Size: 5.6 MB (5565596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c827c09633f3cda18e0cfa5c481bc4d25cdfadc4232d533b82d4f85727ccbd`  
		Last Modified: Thu, 28 Nov 2019 20:26:03 GMT  
		Size: 63.5 MB (63531157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:jre`

```console
$ docker pull ibmjava@sha256:8632798b1e75ac2023a6b444689516cf2b842d52cdbbceb2a55265412ea8aa35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:jre` - linux; amd64

```console
$ docker pull ibmjava@sha256:534f96dcd6dd31abb7e4ef8642446db018310ae282bf400265b3e5320ee84ac6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.9 MB (159902184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f724821d61dbab3904487d424d8e2ade96f509f56cc7df2279982c6019fc53b3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 03:27:18 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 03:27:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:27:26 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 03:28:09 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='31a6f7e851749343cb4fe3956202bdde0beabff901ba926e78cdf013e6d7e725';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='35d0aa5e54b8d68873a2b5de27e834ff4801dcaf598e180b820366f902cef345';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e10ce4e0ba88febefeffef246d59a746c6b9cbe3a3259c792bcf5af807304332';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='bfdb5e450cf4dc9d6f322e8969bb9e7c75d371e38ebf325c635b91ff55eb3ffb';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='3956e363357c68e60c5df1e98a51f75f2e680c237320dea59a02b38e5541ce23';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 03:28:10 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5b7faea59f26f78539055a47552f83601485924313dee5f2d3905977a43aac`  
		Last Modified: Thu, 16 Jan 2020 03:30:20 GMT  
		Size: 3.0 MB (2965136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fed68b301d333ece91cd1852e1757b3b1e70a7db7896318a6dfa3736ff5a3e`  
		Last Modified: Thu, 16 Jan 2020 03:30:32 GMT  
		Size: 130.2 MB (130210480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:jre` - linux; 386

```console
$ docker pull ibmjava@sha256:b55ac8e9ae572334a390204a9a78576fe1c6247aabe4d010fcc9cbbdba6fcace
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.8 MB (148826484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ecba5a21ae87b618ad2a7d5b0d9d9ff261e6e8e8758426e8b3c9b39e0730622`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:38:58 GMT
ADD file:2c41d212af13e7724c6bec90702f30ad85119de23c2ac29494a848e31c568f0f in / 
# Thu, 16 Jan 2020 00:38:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:38:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:39:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:39:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 00:55:58 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 00:56:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:56:07 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 00:56:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='31a6f7e851749343cb4fe3956202bdde0beabff901ba926e78cdf013e6d7e725';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='35d0aa5e54b8d68873a2b5de27e834ff4801dcaf598e180b820366f902cef345';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e10ce4e0ba88febefeffef246d59a746c6b9cbe3a3259c792bcf5af807304332';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='bfdb5e450cf4dc9d6f322e8969bb9e7c75d371e38ebf325c635b91ff55eb3ffb';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='3956e363357c68e60c5df1e98a51f75f2e680c237320dea59a02b38e5541ce23';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 00:56:50 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:0486f132427cc5680d6c6a730e5b518a472f5d0aed43b4c033d3ca9d7f297f21`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 27.1 MB (27122980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884577b2a5cf120bc140e290f06a80bb60802cdc3e0818d2bdb08b724a5a14ef`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 34.6 KB (34620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec417e00c26f6fb4ebd128ca352ab1d4f89b8d9bd06fecdf9a5a64e56c6140b`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c45ceba8ba99dbaa734783259d2a1d46c1ccccbae9bea76e70bbf7629016f5`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8938cf79804632fc6f2701a40497a749ebb1e90d30fec2defad2a8ea1ed872`  
		Last Modified: Thu, 16 Jan 2020 00:58:47 GMT  
		Size: 3.0 MB (2992068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23dcccd16c67a87b392bdc0f10e158d212ca6e0e40a3c23d7b695cd8e60ff23`  
		Last Modified: Thu, 16 Jan 2020 00:58:59 GMT  
		Size: 118.7 MB (118675804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:jre` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:17220ba5d73526dfab8fd9ac4a25b7bc4c503e98f8a05a854eaea0c26bb9e849
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176650569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cba4d0a13eaabd29ca4fe3effacb4896b6a96f1eb757e915bb63a07155b0c18a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:16:57 GMT
ADD file:9a1a27f07b5eac878569b1a3279d14f876400a0bbb293be818f5554662ac82e9 in / 
# Thu, 16 Jan 2020 01:17:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:17:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:17:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:17:19 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:36:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 01:37:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:37:18 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 01:38:22 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='31a6f7e851749343cb4fe3956202bdde0beabff901ba926e78cdf013e6d7e725';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='35d0aa5e54b8d68873a2b5de27e834ff4801dcaf598e180b820366f902cef345';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e10ce4e0ba88febefeffef246d59a746c6b9cbe3a3259c792bcf5af807304332';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='bfdb5e450cf4dc9d6f322e8969bb9e7c75d371e38ebf325c635b91ff55eb3ffb';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='3956e363357c68e60c5df1e98a51f75f2e680c237320dea59a02b38e5541ce23';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 01:38:25 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5592aacf4ac7489bb730c3e5b1799876d68000b7bbf6e9377ca30e16bff059be`  
		Last Modified: Mon, 13 Jan 2020 15:33:24 GMT  
		Size: 30.4 MB (30400610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f7f270f33afb11e2590bebf54c54fcb052048417bc01b24e357117d730d26a`  
		Last Modified: Thu, 16 Jan 2020 01:19:43 GMT  
		Size: 35.2 KB (35217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242585cde72a9805b281397c8fe3b84a8260c6523a4c290da82e6209845c3690`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509fc799f2e0e3149ea8c75fb5b36528e147c5e7123e226d9da46be9c3c79f36`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a14c8ba333672ab64ed6968f103d9a6647e0d49e0789bce7d2a0ebe424b3f5`  
		Last Modified: Thu, 16 Jan 2020 01:41:06 GMT  
		Size: 3.1 MB (3093271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebc985f96c0a80fddf0aa8dc2dc8e4ea2b6e8c213780a630d4e05f25a4a6f28`  
		Last Modified: Thu, 16 Jan 2020 01:41:23 GMT  
		Size: 143.1 MB (143120427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:jre` - linux; s390x

```console
$ docker pull ibmjava@sha256:055430c5163aaeaf101eeff35333202248b9b16790e2ed77d0ec9d39273bfb55
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155583788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3869571e8106ebd89dae543a34aa9b11682ef9e97849d54484afb0fc0b2a6129`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:45:22 GMT
ADD file:4f49a0df2ce5765780345889c57bfaeff1b44de88f7aa876b30ae4f4aa4b1f54 in / 
# Thu, 16 Jan 2020 00:45:23 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:45:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:45:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:45:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:11:09 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 01:11:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:11:15 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 01:11:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='31a6f7e851749343cb4fe3956202bdde0beabff901ba926e78cdf013e6d7e725';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='35d0aa5e54b8d68873a2b5de27e834ff4801dcaf598e180b820366f902cef345';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e10ce4e0ba88febefeffef246d59a746c6b9cbe3a3259c792bcf5af807304332';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='bfdb5e450cf4dc9d6f322e8969bb9e7c75d371e38ebf325c635b91ff55eb3ffb';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='3956e363357c68e60c5df1e98a51f75f2e680c237320dea59a02b38e5541ce23';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 01:11:54 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5e33acada67b43fd81daf3ea8c5b66f480d30d8e6b52e8e3c803d4fe94166024`  
		Last Modified: Mon, 13 Jan 2020 15:34:25 GMT  
		Size: 25.4 MB (25365173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be29508430b95a934d4b70805c50ebe81d716b5aa5b1a3e7d7e674f8c74325dd`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 36.2 KB (36179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed40edcc110aecf91ae3ae074beb10680df57608ad36a93af18548b9c7a49bf2`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f85c1c8cfa969830d1386d6be3d6c989dedcc0a2c65226d4c760a9ec64499b7`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56619e028711aff32431a988d23695bbfd65e0d5f180d8c60579079a24fcedfa`  
		Last Modified: Thu, 16 Jan 2020 01:13:32 GMT  
		Size: 2.7 MB (2678579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d1d179e2201862ab782a8b7943234954684ea1750a3302221d2ee8e7c2360b`  
		Last Modified: Thu, 16 Jan 2020 01:13:42 GMT  
		Size: 127.5 MB (127502848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:jre-alpine`

```console
$ docker pull ibmjava@sha256:2e7f4d0cccf8c3acfe20ae86daf984a8f7f6d13e32622cbff36dbb03d441349a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `ibmjava:jre-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:448e176743d26d21965f9ac27233c9e7467240855f4d2cef95569239ddf5ab12
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138524117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56d0d02bb75b7565fae1266b537cf055a0785626d00f2db2a815ee9ac771db2f`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 17:39:11 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Mon, 21 Oct 2019 17:39:11 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Mon, 21 Oct 2019 17:39:30 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Thu, 28 Nov 2019 20:21:10 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 28 Nov 2019 20:21:50 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='31a6f7e851749343cb4fe3956202bdde0beabff901ba926e78cdf013e6d7e725';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='35d0aa5e54b8d68873a2b5de27e834ff4801dcaf598e180b820366f902cef345';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e10ce4e0ba88febefeffef246d59a746c6b9cbe3a3259c792bcf5af807304332';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='bfdb5e450cf4dc9d6f322e8969bb9e7c75d371e38ebf325c635b91ff55eb3ffb';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='3956e363357c68e60c5df1e98a51f75f2e680c237320dea59a02b38e5541ce23';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Thu, 28 Nov 2019 20:21:50 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd10b3e3ffcf891c3573e370dd214e57c0fc41b96cd920b99f8cb3f118cbbc8`  
		Last Modified: Mon, 21 Oct 2019 17:42:11 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465dff0793d236fe777baf5eb7dd6453017983c9d74ae8aae40ee2a11ba6c369`  
		Last Modified: Mon, 21 Oct 2019 17:42:12 GMT  
		Size: 5.6 MB (5565596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e617b8a4160f048792788dc0a5e4566852cd4c999c23f99fedd388203e1c8b`  
		Last Modified: Thu, 28 Nov 2019 20:25:41 GMT  
		Size: 130.2 MB (130170842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:latest`

```console
$ docker pull ibmjava@sha256:8632798b1e75ac2023a6b444689516cf2b842d52cdbbceb2a55265412ea8aa35
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:latest` - linux; amd64

```console
$ docker pull ibmjava@sha256:534f96dcd6dd31abb7e4ef8642446db018310ae282bf400265b3e5320ee84ac6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.9 MB (159902184 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f724821d61dbab3904487d424d8e2ade96f509f56cc7df2279982c6019fc53b3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 03:27:18 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 03:27:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:27:26 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 03:28:09 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='31a6f7e851749343cb4fe3956202bdde0beabff901ba926e78cdf013e6d7e725';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='35d0aa5e54b8d68873a2b5de27e834ff4801dcaf598e180b820366f902cef345';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e10ce4e0ba88febefeffef246d59a746c6b9cbe3a3259c792bcf5af807304332';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='bfdb5e450cf4dc9d6f322e8969bb9e7c75d371e38ebf325c635b91ff55eb3ffb';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='3956e363357c68e60c5df1e98a51f75f2e680c237320dea59a02b38e5541ce23';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 03:28:10 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5b7faea59f26f78539055a47552f83601485924313dee5f2d3905977a43aac`  
		Last Modified: Thu, 16 Jan 2020 03:30:20 GMT  
		Size: 3.0 MB (2965136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5fed68b301d333ece91cd1852e1757b3b1e70a7db7896318a6dfa3736ff5a3e`  
		Last Modified: Thu, 16 Jan 2020 03:30:32 GMT  
		Size: 130.2 MB (130210480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:latest` - linux; 386

```console
$ docker pull ibmjava@sha256:b55ac8e9ae572334a390204a9a78576fe1c6247aabe4d010fcc9cbbdba6fcace
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.8 MB (148826484 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ecba5a21ae87b618ad2a7d5b0d9d9ff261e6e8e8758426e8b3c9b39e0730622`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:38:58 GMT
ADD file:2c41d212af13e7724c6bec90702f30ad85119de23c2ac29494a848e31c568f0f in / 
# Thu, 16 Jan 2020 00:38:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:38:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:39:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:39:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 00:55:58 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 00:56:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:56:07 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 00:56:50 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='31a6f7e851749343cb4fe3956202bdde0beabff901ba926e78cdf013e6d7e725';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='35d0aa5e54b8d68873a2b5de27e834ff4801dcaf598e180b820366f902cef345';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e10ce4e0ba88febefeffef246d59a746c6b9cbe3a3259c792bcf5af807304332';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='bfdb5e450cf4dc9d6f322e8969bb9e7c75d371e38ebf325c635b91ff55eb3ffb';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='3956e363357c68e60c5df1e98a51f75f2e680c237320dea59a02b38e5541ce23';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 00:56:50 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:0486f132427cc5680d6c6a730e5b518a472f5d0aed43b4c033d3ca9d7f297f21`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 27.1 MB (27122980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884577b2a5cf120bc140e290f06a80bb60802cdc3e0818d2bdb08b724a5a14ef`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 34.6 KB (34620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec417e00c26f6fb4ebd128ca352ab1d4f89b8d9bd06fecdf9a5a64e56c6140b`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c45ceba8ba99dbaa734783259d2a1d46c1ccccbae9bea76e70bbf7629016f5`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8938cf79804632fc6f2701a40497a749ebb1e90d30fec2defad2a8ea1ed872`  
		Last Modified: Thu, 16 Jan 2020 00:58:47 GMT  
		Size: 3.0 MB (2992068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23dcccd16c67a87b392bdc0f10e158d212ca6e0e40a3c23d7b695cd8e60ff23`  
		Last Modified: Thu, 16 Jan 2020 00:58:59 GMT  
		Size: 118.7 MB (118675804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:latest` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:17220ba5d73526dfab8fd9ac4a25b7bc4c503e98f8a05a854eaea0c26bb9e849
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.7 MB (176650569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cba4d0a13eaabd29ca4fe3effacb4896b6a96f1eb757e915bb63a07155b0c18a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:16:57 GMT
ADD file:9a1a27f07b5eac878569b1a3279d14f876400a0bbb293be818f5554662ac82e9 in / 
# Thu, 16 Jan 2020 01:17:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:17:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:17:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:17:19 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:36:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 01:37:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:37:18 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 01:38:22 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='31a6f7e851749343cb4fe3956202bdde0beabff901ba926e78cdf013e6d7e725';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='35d0aa5e54b8d68873a2b5de27e834ff4801dcaf598e180b820366f902cef345';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e10ce4e0ba88febefeffef246d59a746c6b9cbe3a3259c792bcf5af807304332';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='bfdb5e450cf4dc9d6f322e8969bb9e7c75d371e38ebf325c635b91ff55eb3ffb';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='3956e363357c68e60c5df1e98a51f75f2e680c237320dea59a02b38e5541ce23';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 01:38:25 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5592aacf4ac7489bb730c3e5b1799876d68000b7bbf6e9377ca30e16bff059be`  
		Last Modified: Mon, 13 Jan 2020 15:33:24 GMT  
		Size: 30.4 MB (30400610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f7f270f33afb11e2590bebf54c54fcb052048417bc01b24e357117d730d26a`  
		Last Modified: Thu, 16 Jan 2020 01:19:43 GMT  
		Size: 35.2 KB (35217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242585cde72a9805b281397c8fe3b84a8260c6523a4c290da82e6209845c3690`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509fc799f2e0e3149ea8c75fb5b36528e147c5e7123e226d9da46be9c3c79f36`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a14c8ba333672ab64ed6968f103d9a6647e0d49e0789bce7d2a0ebe424b3f5`  
		Last Modified: Thu, 16 Jan 2020 01:41:06 GMT  
		Size: 3.1 MB (3093271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebc985f96c0a80fddf0aa8dc2dc8e4ea2b6e8c213780a630d4e05f25a4a6f28`  
		Last Modified: Thu, 16 Jan 2020 01:41:23 GMT  
		Size: 143.1 MB (143120427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:latest` - linux; s390x

```console
$ docker pull ibmjava@sha256:055430c5163aaeaf101eeff35333202248b9b16790e2ed77d0ec9d39273bfb55
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155583788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3869571e8106ebd89dae543a34aa9b11682ef9e97849d54484afb0fc0b2a6129`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:45:22 GMT
ADD file:4f49a0df2ce5765780345889c57bfaeff1b44de88f7aa876b30ae4f4aa4b1f54 in / 
# Thu, 16 Jan 2020 00:45:23 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:45:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:45:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:45:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:11:09 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 01:11:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:11:15 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 01:11:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='31a6f7e851749343cb4fe3956202bdde0beabff901ba926e78cdf013e6d7e725';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='35d0aa5e54b8d68873a2b5de27e834ff4801dcaf598e180b820366f902cef345';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='e10ce4e0ba88febefeffef246d59a746c6b9cbe3a3259c792bcf5af807304332';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='bfdb5e450cf4dc9d6f322e8969bb9e7c75d371e38ebf325c635b91ff55eb3ffb';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='3956e363357c68e60c5df1e98a51f75f2e680c237320dea59a02b38e5541ce23';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 01:11:54 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5e33acada67b43fd81daf3ea8c5b66f480d30d8e6b52e8e3c803d4fe94166024`  
		Last Modified: Mon, 13 Jan 2020 15:34:25 GMT  
		Size: 25.4 MB (25365173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be29508430b95a934d4b70805c50ebe81d716b5aa5b1a3e7d7e674f8c74325dd`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 36.2 KB (36179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed40edcc110aecf91ae3ae074beb10680df57608ad36a93af18548b9c7a49bf2`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f85c1c8cfa969830d1386d6be3d6c989dedcc0a2c65226d4c760a9ec64499b7`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56619e028711aff32431a988d23695bbfd65e0d5f180d8c60579079a24fcedfa`  
		Last Modified: Thu, 16 Jan 2020 01:13:32 GMT  
		Size: 2.7 MB (2678579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d1d179e2201862ab782a8b7943234954684ea1750a3302221d2ee8e7c2360b`  
		Last Modified: Thu, 16 Jan 2020 01:13:42 GMT  
		Size: 127.5 MB (127502848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:sdk`

```console
$ docker pull ibmjava@sha256:9b27a9d9c33e484f25bd4ff71ca5e19c4ebc1bc2b9606392ac02fb7bf279ed9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:sdk` - linux; amd64

```console
$ docker pull ibmjava@sha256:2eb69e6b419e6ccb51201bf7913bd7a70c6cb8fe29458f424a75ea5467a2de36
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.1 MB (197062481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6916b880c33ec4b03b8172bd6056e1fb5204a70140334ebefbe95236e041dec0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 03:27:18 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 03:27:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:27:26 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 03:29:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='4c3b62dc988223239d0049e03c40444524356e3cdf805972e1a35d127d00c1c9';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='8618f9ed7bd5575f17ea9e63d8c37f2afa283bf6c9c240bd6f7eba18642c1227';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='18c2eccf99225e6e7643141d8da4110cacc39f2fa00149fc26341d2272cc0102';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='095f80d219f95158e1b734d1632b40dc1aaa457fd04e23e04e6e9667adc8bf48';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='97e45a2fffa1ec8c57da614313cbb32d430210ae18e22c7022cd18204ea5ec96';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 03:29:58 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5b7faea59f26f78539055a47552f83601485924313dee5f2d3905977a43aac`  
		Last Modified: Thu, 16 Jan 2020 03:30:20 GMT  
		Size: 3.0 MB (2965136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821c49691759d482d6d0ba4f40279447943769f0e477d9b4f2e2e65af884bb2e`  
		Last Modified: Thu, 16 Jan 2020 03:31:08 GMT  
		Size: 167.4 MB (167370777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sdk` - linux; 386

```console
$ docker pull ibmjava@sha256:fdfbcbababd489a0feba701d2f75d92a4d50a441f4cf2d546c3d16e1377828a4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.9 MB (185874249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df8fe399784d565a9f6b8894520c0f5f8f9c2bf4e3951a5e3b587c5a4b67133f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:38:58 GMT
ADD file:2c41d212af13e7724c6bec90702f30ad85119de23c2ac29494a848e31c568f0f in / 
# Thu, 16 Jan 2020 00:38:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:38:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:39:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:39:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 00:55:58 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 00:56:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:56:07 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 00:58:29 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='4c3b62dc988223239d0049e03c40444524356e3cdf805972e1a35d127d00c1c9';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='8618f9ed7bd5575f17ea9e63d8c37f2afa283bf6c9c240bd6f7eba18642c1227';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='18c2eccf99225e6e7643141d8da4110cacc39f2fa00149fc26341d2272cc0102';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='095f80d219f95158e1b734d1632b40dc1aaa457fd04e23e04e6e9667adc8bf48';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='97e45a2fffa1ec8c57da614313cbb32d430210ae18e22c7022cd18204ea5ec96';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 00:58:30 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:0486f132427cc5680d6c6a730e5b518a472f5d0aed43b4c033d3ca9d7f297f21`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 27.1 MB (27122980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884577b2a5cf120bc140e290f06a80bb60802cdc3e0818d2bdb08b724a5a14ef`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 34.6 KB (34620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec417e00c26f6fb4ebd128ca352ab1d4f89b8d9bd06fecdf9a5a64e56c6140b`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c45ceba8ba99dbaa734783259d2a1d46c1ccccbae9bea76e70bbf7629016f5`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8938cf79804632fc6f2701a40497a749ebb1e90d30fec2defad2a8ea1ed872`  
		Last Modified: Thu, 16 Jan 2020 00:58:47 GMT  
		Size: 3.0 MB (2992068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:426f3d330e3eea8713e33b004242816bcf884f9eb046e03ca4f66289441458a7`  
		Last Modified: Thu, 16 Jan 2020 00:59:50 GMT  
		Size: 155.7 MB (155723569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sdk` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:1f35a2bccb16bf654639e48f32729bc6f940c76074d3151a2908c4db5342722f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **213.9 MB (213928209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a6d6449090b49333e2e3f800f4e19b7456de1e90359caf5b5a0d20b600d1bef`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:16:57 GMT
ADD file:9a1a27f07b5eac878569b1a3279d14f876400a0bbb293be818f5554662ac82e9 in / 
# Thu, 16 Jan 2020 01:17:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:17:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:17:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:17:19 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:36:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 01:37:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:37:18 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 01:40:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='4c3b62dc988223239d0049e03c40444524356e3cdf805972e1a35d127d00c1c9';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='8618f9ed7bd5575f17ea9e63d8c37f2afa283bf6c9c240bd6f7eba18642c1227';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='18c2eccf99225e6e7643141d8da4110cacc39f2fa00149fc26341d2272cc0102';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='095f80d219f95158e1b734d1632b40dc1aaa457fd04e23e04e6e9667adc8bf48';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='97e45a2fffa1ec8c57da614313cbb32d430210ae18e22c7022cd18204ea5ec96';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 01:40:48 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5592aacf4ac7489bb730c3e5b1799876d68000b7bbf6e9377ca30e16bff059be`  
		Last Modified: Mon, 13 Jan 2020 15:33:24 GMT  
		Size: 30.4 MB (30400610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f7f270f33afb11e2590bebf54c54fcb052048417bc01b24e357117d730d26a`  
		Last Modified: Thu, 16 Jan 2020 01:19:43 GMT  
		Size: 35.2 KB (35217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242585cde72a9805b281397c8fe3b84a8260c6523a4c290da82e6209845c3690`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509fc799f2e0e3149ea8c75fb5b36528e147c5e7123e226d9da46be9c3c79f36`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a14c8ba333672ab64ed6968f103d9a6647e0d49e0789bce7d2a0ebe424b3f5`  
		Last Modified: Thu, 16 Jan 2020 01:41:06 GMT  
		Size: 3.1 MB (3093271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e610c730b6954c1f9636195c0e065064a88c1f0a365feacb864a7b1fdff230`  
		Last Modified: Thu, 16 Jan 2020 01:42:47 GMT  
		Size: 180.4 MB (180398067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sdk` - linux; s390x

```console
$ docker pull ibmjava@sha256:bc4984ac270a50360519efb0e514297ccdca2ed333624a2d4f238d8b6a0844ff
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.8 MB (185829502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1f7dad284aac0e12062652652f3a10ddb45f397a1306e70307dd503bcc85e72`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:45:22 GMT
ADD file:4f49a0df2ce5765780345889c57bfaeff1b44de88f7aa876b30ae4f4aa4b1f54 in / 
# Thu, 16 Jan 2020 00:45:23 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:45:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:45:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:45:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:11:09 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 01:11:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:11:15 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 01:13:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='4c3b62dc988223239d0049e03c40444524356e3cdf805972e1a35d127d00c1c9';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='8618f9ed7bd5575f17ea9e63d8c37f2afa283bf6c9c240bd6f7eba18642c1227';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='18c2eccf99225e6e7643141d8da4110cacc39f2fa00149fc26341d2272cc0102';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='095f80d219f95158e1b734d1632b40dc1aaa457fd04e23e04e6e9667adc8bf48';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='97e45a2fffa1ec8c57da614313cbb32d430210ae18e22c7022cd18204ea5ec96';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 01:13:23 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5e33acada67b43fd81daf3ea8c5b66f480d30d8e6b52e8e3c803d4fe94166024`  
		Last Modified: Mon, 13 Jan 2020 15:34:25 GMT  
		Size: 25.4 MB (25365173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be29508430b95a934d4b70805c50ebe81d716b5aa5b1a3e7d7e674f8c74325dd`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 36.2 KB (36179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed40edcc110aecf91ae3ae074beb10680df57608ad36a93af18548b9c7a49bf2`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f85c1c8cfa969830d1386d6be3d6c989dedcc0a2c65226d4c760a9ec64499b7`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56619e028711aff32431a988d23695bbfd65e0d5f180d8c60579079a24fcedfa`  
		Last Modified: Thu, 16 Jan 2020 01:13:32 GMT  
		Size: 2.7 MB (2678579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e0d8fc0c0bc62dab86f7c970fd715f47f4969931df1563d7840df76a9b3e15`  
		Last Modified: Thu, 16 Jan 2020 01:14:11 GMT  
		Size: 157.7 MB (157748562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:sdk-alpine`

```console
$ docker pull ibmjava@sha256:90199ebb409616ca8b538efea2ad290b5835876649ac23fbb3e674694498edb6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `ibmjava:sdk-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:c7edb4c364882cfef4ac405cbb65e6fd936cfde5ad2b554ac7c6a30dca41d867
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.7 MB (175679272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:675ab2389e990d2b76715850754687213245217e7720c90677bf731f2e852aaf`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 17:39:11 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Mon, 21 Oct 2019 17:39:11 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Mon, 21 Oct 2019 17:39:30 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Thu, 28 Nov 2019 20:21:10 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 28 Nov 2019 20:24:59 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='4c3b62dc988223239d0049e03c40444524356e3cdf805972e1a35d127d00c1c9';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='8618f9ed7bd5575f17ea9e63d8c37f2afa283bf6c9c240bd6f7eba18642c1227';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='18c2eccf99225e6e7643141d8da4110cacc39f2fa00149fc26341d2272cc0102';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='095f80d219f95158e1b734d1632b40dc1aaa457fd04e23e04e6e9667adc8bf48';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='97e45a2fffa1ec8c57da614313cbb32d430210ae18e22c7022cd18204ea5ec96';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Thu, 28 Nov 2019 20:24:59 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd10b3e3ffcf891c3573e370dd214e57c0fc41b96cd920b99f8cb3f118cbbc8`  
		Last Modified: Mon, 21 Oct 2019 17:42:11 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465dff0793d236fe777baf5eb7dd6453017983c9d74ae8aae40ee2a11ba6c369`  
		Last Modified: Mon, 21 Oct 2019 17:42:12 GMT  
		Size: 5.6 MB (5565596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25ea3903d89773e915cc11ad7083d8d6c04c8ed4b3623a0f628a1721a0f51831`  
		Last Modified: Thu, 28 Nov 2019 20:26:46 GMT  
		Size: 167.3 MB (167325997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:sfj`

```console
$ docker pull ibmjava@sha256:287008706919354c0fc9b4f93edfdf7fedcd74e87641405da2acc0974a08e52e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:sfj` - linux; amd64

```console
$ docker pull ibmjava@sha256:8767aebf1906a826a198dc5db305747c7fa2e449fdf1e73800a28a2ebf5baad2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93210577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3564b44cc8e2dc75197cc0e9ddcdb99699b0b1aa1d508a3a1dc8569e7b86e75`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:20:31 GMT
ADD file:08e718ed0796013f5957a1be7da3bef6225f3d82d8be0a86a7114e5caad50cbc in / 
# Thu, 16 Jan 2020 01:20:32 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:20:33 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:20:34 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:20:34 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 03:27:18 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 03:27:26 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 03:27:26 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 03:28:58 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='822b2bd8286c2ec4a7dd7f84386be3ccf43f0f1c3e259c4ed96aac3210d3e11a';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='4147cb108ea191199ca86d298692d87381f354ce0b15e22c2bcadc0f49a1af4a';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='fbe53ee7151f624b6119106373115d319554cc1760b32dee6c37113157d1c773';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='cc0b10e220eca7e6c76a2d461018055e2e41e0f532d8ddf08c7dd7eb06770f14';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='81962223b3e439e2d9a8e38b51ffc5f80f18884216fd41647192baebf4829708';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 03:28:58 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5c939e3a4d1097af8d3292ad3a41d3caa846f6333b91f2dd22b972bc2d19c5b5`  
		Last Modified: Mon, 13 Jan 2020 13:21:09 GMT  
		Size: 26.7 MB (26690191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c63719cdbe7ae254b453dba06fb446f583b503f2a2c15becc83f8c5bc7a705e0`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 35.4 KB (35366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a861ea6baff71b05cd577478984c3e62cf0177bf74468d0aca551f5fcb891c`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:651c9d2d6c4f37c56a221259e033e7e2353b698139c2ff950623ca28d64a9837`  
		Last Modified: Thu, 16 Jan 2020 01:21:44 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5b7faea59f26f78539055a47552f83601485924313dee5f2d3905977a43aac`  
		Last Modified: Thu, 16 Jan 2020 03:30:20 GMT  
		Size: 3.0 MB (2965136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff65401a9d7a35b6c3ad2220d1593d6406450066542fd5b3683fb96b84ffa357`  
		Last Modified: Thu, 16 Jan 2020 03:30:50 GMT  
		Size: 63.5 MB (63518873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; 386

```console
$ docker pull ibmjava@sha256:9b7f8545ce9c2e84cb1e274a853546f7e7788310df00a9a63150f55ca64a1123
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93095310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92e652d0abed34825e3a6ebf618d0b850870fa1fb76162bef773b3de3d778bd0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:38:58 GMT
ADD file:2c41d212af13e7724c6bec90702f30ad85119de23c2ac29494a848e31c568f0f in / 
# Thu, 16 Jan 2020 00:38:58 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:38:59 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:39:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:39:00 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 00:55:58 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 00:56:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 00:56:07 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 00:57:34 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='822b2bd8286c2ec4a7dd7f84386be3ccf43f0f1c3e259c4ed96aac3210d3e11a';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='4147cb108ea191199ca86d298692d87381f354ce0b15e22c2bcadc0f49a1af4a';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='fbe53ee7151f624b6119106373115d319554cc1760b32dee6c37113157d1c773';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='cc0b10e220eca7e6c76a2d461018055e2e41e0f532d8ddf08c7dd7eb06770f14';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='81962223b3e439e2d9a8e38b51ffc5f80f18884216fd41647192baebf4829708';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 00:57:34 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:0486f132427cc5680d6c6a730e5b518a472f5d0aed43b4c033d3ca9d7f297f21`  
		Last Modified: Mon, 13 Jan 2020 15:33:17 GMT  
		Size: 27.1 MB (27122980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884577b2a5cf120bc140e290f06a80bb60802cdc3e0818d2bdb08b724a5a14ef`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 34.6 KB (34620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec417e00c26f6fb4ebd128ca352ab1d4f89b8d9bd06fecdf9a5a64e56c6140b`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87c45ceba8ba99dbaa734783259d2a1d46c1ccccbae9bea76e70bbf7629016f5`  
		Last Modified: Thu, 16 Jan 2020 00:39:53 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8938cf79804632fc6f2701a40497a749ebb1e90d30fec2defad2a8ea1ed872`  
		Last Modified: Thu, 16 Jan 2020 00:58:47 GMT  
		Size: 3.0 MB (2992068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1ce2aa2cc3d5e869c33a184a1345a9cd9084f7b9e6a0d2ac4075e06c1847f6`  
		Last Modified: Thu, 16 Jan 2020 00:59:14 GMT  
		Size: 62.9 MB (62944630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:f973cc82219c07335a2b02a465b31ce90e03dcdc2f1315e1049eb248e1dab406
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.6 MB (101639936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c61b6e68f1c1f6f7c31db6fda5112d80a2d09b823ef62fc4fce3e14cd56c705`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 01:16:57 GMT
ADD file:9a1a27f07b5eac878569b1a3279d14f876400a0bbb293be818f5554662ac82e9 in / 
# Thu, 16 Jan 2020 01:17:05 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 01:17:10 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 01:17:17 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 01:17:19 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:36:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 01:37:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:37:18 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 01:39:15 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='822b2bd8286c2ec4a7dd7f84386be3ccf43f0f1c3e259c4ed96aac3210d3e11a';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='4147cb108ea191199ca86d298692d87381f354ce0b15e22c2bcadc0f49a1af4a';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='fbe53ee7151f624b6119106373115d319554cc1760b32dee6c37113157d1c773';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='cc0b10e220eca7e6c76a2d461018055e2e41e0f532d8ddf08c7dd7eb06770f14';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='81962223b3e439e2d9a8e38b51ffc5f80f18884216fd41647192baebf4829708';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 01:39:19 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5592aacf4ac7489bb730c3e5b1799876d68000b7bbf6e9377ca30e16bff059be`  
		Last Modified: Mon, 13 Jan 2020 15:33:24 GMT  
		Size: 30.4 MB (30400610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f7f270f33afb11e2590bebf54c54fcb052048417bc01b24e357117d730d26a`  
		Last Modified: Thu, 16 Jan 2020 01:19:43 GMT  
		Size: 35.2 KB (35217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242585cde72a9805b281397c8fe3b84a8260c6523a4c290da82e6209845c3690`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509fc799f2e0e3149ea8c75fb5b36528e147c5e7123e226d9da46be9c3c79f36`  
		Last Modified: Thu, 16 Jan 2020 01:19:42 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a14c8ba333672ab64ed6968f103d9a6647e0d49e0789bce7d2a0ebe424b3f5`  
		Last Modified: Thu, 16 Jan 2020 01:41:06 GMT  
		Size: 3.1 MB (3093271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:227a44da282b869228b869e8a9c2b5f3a83403eb47d9219a37712d92e5d51d2c`  
		Last Modified: Thu, 16 Jan 2020 01:41:49 GMT  
		Size: 68.1 MB (68109794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; s390x

```console
$ docker pull ibmjava@sha256:fc47a4bd11377cfa3debbd1939cbf28481ae9a067ebc06200abccdb4a0c508cb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.8 MB (92776886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c579628c5b6fb6357794b06aff9f90319869f8b90426c1d80c88613169d27615`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 16 Jan 2020 00:45:22 GMT
ADD file:4f49a0df2ce5765780345889c57bfaeff1b44de88f7aa876b30ae4f4aa4b1f54 in / 
# Thu, 16 Jan 2020 00:45:23 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Thu, 16 Jan 2020 00:45:23 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Thu, 16 Jan 2020 00:45:24 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Thu, 16 Jan 2020 00:45:24 GMT
CMD ["/bin/bash"]
# Thu, 16 Jan 2020 01:11:09 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 16 Jan 2020 01:11:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 16 Jan 2020 01:11:15 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 16 Jan 2020 01:12:33 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='822b2bd8286c2ec4a7dd7f84386be3ccf43f0f1c3e259c4ed96aac3210d3e11a';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='4147cb108ea191199ca86d298692d87381f354ce0b15e22c2bcadc0f49a1af4a';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='fbe53ee7151f624b6119106373115d319554cc1760b32dee6c37113157d1c773';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='cc0b10e220eca7e6c76a2d461018055e2e41e0f532d8ddf08c7dd7eb06770f14';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='81962223b3e439e2d9a8e38b51ffc5f80f18884216fd41647192baebf4829708';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 16 Jan 2020 01:12:33 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:5e33acada67b43fd81daf3ea8c5b66f480d30d8e6b52e8e3c803d4fe94166024`  
		Last Modified: Mon, 13 Jan 2020 15:34:25 GMT  
		Size: 25.4 MB (25365173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be29508430b95a934d4b70805c50ebe81d716b5aa5b1a3e7d7e674f8c74325dd`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 36.2 KB (36179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed40edcc110aecf91ae3ae074beb10680df57608ad36a93af18548b9c7a49bf2`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f85c1c8cfa969830d1386d6be3d6c989dedcc0a2c65226d4c760a9ec64499b7`  
		Last Modified: Thu, 16 Jan 2020 00:46:10 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56619e028711aff32431a988d23695bbfd65e0d5f180d8c60579079a24fcedfa`  
		Last Modified: Thu, 16 Jan 2020 01:13:32 GMT  
		Size: 2.7 MB (2678579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd0bb0ee417b74a1fdc0d4cbb7d3f8eeab02bd9d9366220e23e4e1139c319c32`  
		Last Modified: Thu, 16 Jan 2020 01:13:55 GMT  
		Size: 64.7 MB (64695946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:sfj-alpine`

```console
$ docker pull ibmjava@sha256:2f266d2e5e9c15d7ad0a572e87109d8d644ffc05827c50b3b998e0bc5e8cf836
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `ibmjava:sfj-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:f019479be9bc7942a52a9b72a2a5fadf2d4a770ae875b42e44c0c7d40798ce91
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71884432 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:793e22b65549745e55f78b6a266575c26aba2ef71b71e84ac11342257d0dd3c0`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 17:39:11 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Mon, 21 Oct 2019 17:39:11 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Mon, 21 Oct 2019 17:39:30 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Thu, 28 Nov 2019 20:21:10 GMT
ENV JAVA_VERSION=1.8.0_sr6
# Thu, 28 Nov 2019 20:23:03 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='822b2bd8286c2ec4a7dd7f84386be3ccf43f0f1c3e259c4ed96aac3210d3e11a';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='4147cb108ea191199ca86d298692d87381f354ce0b15e22c2bcadc0f49a1af4a';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='fbe53ee7151f624b6119106373115d319554cc1760b32dee6c37113157d1c773';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='cc0b10e220eca7e6c76a2d461018055e2e41e0f532d8ddf08c7dd7eb06770f14';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='81962223b3e439e2d9a8e38b51ffc5f80f18884216fd41647192baebf4829708';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Thu, 28 Nov 2019 20:23:03 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd10b3e3ffcf891c3573e370dd214e57c0fc41b96cd920b99f8cb3f118cbbc8`  
		Last Modified: Mon, 21 Oct 2019 17:42:11 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465dff0793d236fe777baf5eb7dd6453017983c9d74ae8aae40ee2a11ba6c369`  
		Last Modified: Mon, 21 Oct 2019 17:42:12 GMT  
		Size: 5.6 MB (5565596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c827c09633f3cda18e0cfa5c481bc4d25cdfadc4232d533b82d4f85727ccbd`  
		Last Modified: Thu, 28 Nov 2019 20:26:03 GMT  
		Size: 63.5 MB (63531157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
