## `ibmjava:jre`

```console
$ docker pull ibmjava@sha256:df95fc05dad532110d53dda8551bada89c4cb1363e8aecb8e7ed54c7839d7992
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:jre` - linux; amd64

```console
$ docker pull ibmjava@sha256:f33852b6c01f666cc19d908e02391b7f3d288c7b36dd5ca4049b1ef9950b29cc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.0 MB (160032634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf558863311e132f4ab3b59cc7e41930ed48324a06cef579642dafbc1abc78ff`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:38:19 GMT
ADD file:7d9bbf45a5b2510d44d3206a028cf6502757884d49e46d3d2e6356c3a92c4309 in / 
# Fri, 24 Jul 2020 14:38:20 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:38:21 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:38:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:38:22 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 16:11:53 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 16:12:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 16:12:01 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 16:12:44 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 16:12:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:7595c8c21622ea8a8b9778972e26dbbe063f7a1c4b0a28a80a34ebb3d343b586`  
		Last Modified: Mon, 13 Jul 2020 15:46:50 GMT  
		Size: 26.7 MB (26697127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13af8ca898f36af68711cb67c345f65046a78ccd802453f4b129adf9205b1f8`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 35.4 KB (35364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70799171ddba93a611490ba3557d782714b3f4da8963d49ac8726786ba8274a5`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6c12202c5ef07dc9eb8f9d9e71407064684ed70f8c4040b62679b7d30200840`  
		Last Modified: Fri, 24 Jul 2020 14:39:21 GMT  
		Size: 161.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3b48ae14e45cf7769bcc5ef96dd1a0d4389a21fd1de5c54169068b1730e569`  
		Last Modified: Fri, 24 Jul 2020 16:14:39 GMT  
		Size: 3.0 MB (2957372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb345f3aba04dd4cc154f33e9bfd3ece70843c13b3d997ea5736dab388e4b6b8`  
		Last Modified: Fri, 24 Jul 2020 16:14:50 GMT  
		Size: 130.3 MB (130341762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:jre` - linux; 386

```console
$ docker pull ibmjava@sha256:84b58f3339f1ab7b90e8cca32557508d3c62de627513a41bd65478f4b4486e7c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.8 MB (148849649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0e4a395028813b1758de54169a9063ebed57557d679fba2364c5079d2b6edac`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:40:18 GMT
ADD file:1041a59a13c0d49b1cb87f211694f68be4c9b76f2deb36e2d8955b77c4d2836f in / 
# Fri, 24 Jul 2020 14:40:19 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:40:20 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:40:21 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:40:21 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 14:56:28 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 14:56:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 14:56:40 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 14:57:23 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 14:57:23 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:89823af3b784a3ef6d57a90159cbd5f28c863927aa03d4c43b44b6c37479fa1c`  
		Last Modified: Mon, 13 Jul 2020 15:46:56 GMT  
		Size: 27.1 MB (27123624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28677484c2569b014ecb876df3111b11e825c82629306b3af99a1c12f3b234e2`  
		Last Modified: Fri, 24 Jul 2020 14:40:50 GMT  
		Size: 34.6 KB (34611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c914b15d9c03339769ddd662b893654bbc371dbed4f8cdfa29ca1c57c0bb98e`  
		Last Modified: Fri, 24 Jul 2020 14:40:50 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9dc7dbf6d65bca5959e6f7c892f468288c27e6a0ef07eec142d4497ee07e6cd`  
		Last Modified: Fri, 24 Jul 2020 14:40:50 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6390acddeaf0d5abd6917da9b4934d31bc7973be5b9dceb484774c00312c178`  
		Last Modified: Fri, 24 Jul 2020 14:59:13 GMT  
		Size: 3.0 MB (2982896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b177f3853d875c18d17b4e8f702b7a1748b053c1ef83d54efd67ab2f8450ac6`  
		Last Modified: Fri, 24 Jul 2020 14:59:27 GMT  
		Size: 118.7 MB (118707507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:jre` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:88f999aa4181c30408049102193b5ae745fcf80412fdf1709d3b49f2eec38f63
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.4 MB (172355108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51912a4ac2b5af0bb1d292f68a2c042ef7d642ea21204227fcdb049dce01d883`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:33:42 GMT
ADD file:d8c73324b090ba968a3efc4afc8af7d913766bd7787fc4cd6e4436895a4e564a in / 
# Fri, 24 Jul 2020 14:34:10 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:34:45 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:35:00 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:35:08 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 17:20:40 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 17:21:29 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 17:21:38 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 17:23:01 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 17:23:23 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:453712c8810fcce792c21167e028047a35328679a3bd4429b8837301315e9103`  
		Last Modified: Mon, 13 Jul 2020 15:47:10 GMT  
		Size: 30.4 MB (30404926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecbb4638d99213e93a32d6945492539426ee3616d7ba413462a8b936268a56af`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 35.2 KB (35224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b0bd277b733224c67d835643aa13dd8a9b86bcc10023a393302b3861e9a7b8`  
		Last Modified: Fri, 24 Jul 2020 14:41:32 GMT  
		Size: 853.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:270c2b729d72bf4931bb8d6ccbd100e124e01bac9628380f36c2d0f13bdcc109`  
		Last Modified: Fri, 24 Jul 2020 14:41:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8989d267f52940d635da8bfa3e6956dcffdc261b063087c2c5d94aa80c19c32`  
		Last Modified: Fri, 24 Jul 2020 17:27:23 GMT  
		Size: 3.1 MB (3075410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debab8a113f0c1af82b60f886849e4c99bd273d6f24c8939febce35e08ac4cf2`  
		Last Modified: Fri, 24 Jul 2020 17:27:37 GMT  
		Size: 138.8 MB (138838507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:jre` - linux; s390x

```console
$ docker pull ibmjava@sha256:9428c46ceb67efdcf0e61393d9dff6ed2efd58a6346c5314f6c866c2fd764265
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.7 MB (155680443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a291ce4db9a17a350d0afb0fdfa36422272d64bb40c75ae2ae776d7bdfd7213`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 24 Jul 2020 14:43:52 GMT
ADD file:03965719c666ec8be956f87c8fd8121313110d14fd14f25a85be1281e4ca000b in / 
# Fri, 24 Jul 2020 14:44:00 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 24 Jul 2020 14:44:02 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 24 Jul 2020 14:44:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 24 Jul 2020 14:44:05 GMT
CMD ["/bin/bash"]
# Fri, 24 Jul 2020 15:01:51 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 24 Jul 2020 15:02:07 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 24 Jul 2020 15:02:08 GMT
ENV JAVA_VERSION=1.8.0_sr6fp11
# Fri, 24 Jul 2020 15:03:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='e318577a2c807fd515129c96b10e86c9ea2f8318a74d2ac54d53ff9fd85450cc';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='708960c09d456e1b84b7caf0000995fc266af90cbcb6ca053bee0d19c625d5a6';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='43a40e8d1164e0904ef0a91100d4a6579e4075f6ea503a417d4122c4c1321f22';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='570cec9a573a1b849db8b8f5485813fce7a384c6de6090eec93e4427244aa5af';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='c9f43396f318f73bcb40f652a40debbb1cef83f36c3f3fc7cf03d5fcbdfd48c2';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 24 Jul 2020 15:03:14 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:be08d3c199ef98c9593e956954bc77a9dbc438573a70702d7b3464d4e8d1ac41`  
		Last Modified: Mon, 13 Jul 2020 15:48:28 GMT  
		Size: 25.4 MB (25369527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d13cd4fc4b78e5f1f87dd7f9b563a260a4a858377937981e98c3246b6908cf`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 36.2 KB (36170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b49d28fc51a8e47b741fef4363cbf334000d3955d4bdef76622a0a5ba72a88`  
		Last Modified: Fri, 24 Jul 2020 14:45:31 GMT  
		Size: 848.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e784976bb1b84890c7c9256bdf2d9d634bc901a832f0724a5cf6d1e365e44f`  
		Last Modified: Fri, 24 Jul 2020 14:45:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0a405adecbf26fa229b5a95f8e8bf05751335fb161fd163398048a3b477ee38`  
		Last Modified: Fri, 24 Jul 2020 15:05:54 GMT  
		Size: 2.7 MB (2672379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81fb774239222293784df8b9f247962c4940509522a4fc4e0d7d97066e4a612b`  
		Last Modified: Fri, 24 Jul 2020 15:06:09 GMT  
		Size: 127.6 MB (127601331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
