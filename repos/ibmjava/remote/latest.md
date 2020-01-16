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
