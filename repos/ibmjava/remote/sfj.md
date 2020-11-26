## `ibmjava:sfj`

```console
$ docker pull ibmjava@sha256:e08498366620a7a6adba6cd5e0804f04e8f898b9679a6a0660bbe4415643f9cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:sfj` - linux; amd64

```console
$ docker pull ibmjava@sha256:6ce0758d1b2e89b395cf5c8114a057ba402440f6cad7c496e200c48f42efab6e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93176122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edc4992a6cebdf70c81c142effe9ab8cb25c0bf91980740e259251b2c421bc50`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Nov 2020 22:25:13 GMT
ADD file:6ef542de9959c3061f2d0758adb031e226b221a1a2cd748ff59e6fc13216a1c0 in / 
# Wed, 25 Nov 2020 22:25:14 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:25:15 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:25:16 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:25:17 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 23:12:02 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 25 Nov 2020 23:12:17 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 23:12:17 GMT
ENV JAVA_VERSION=1.8.0_sr6fp16
# Wed, 25 Nov 2020 23:13:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d143836caa7e7777f6bf4539b249c48341da97ca4d27f012cf5541b35376e479';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='104b7d07afb812acf1d37a1409cf9dbf360745f346a50a3954ae465315966ad5';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='d2d5ca9484d0801816a74b66551a07d5f69fb41e52aeb5f10ddf1d55c1a46d06';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='dd5d853e9dbbcd7342c7dfb0259b675b951ae1faadbbb667f6553270ceb5b4f8';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='a4b617ba4614317f92159a6930a7ae369923b909377a4d0f2aff9ce3b098ac39';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 25 Nov 2020 23:13:57 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:f22ccc0b8772d8e1bcb40f137b373686bc27427a70c0e41dd22b38016e09e7e0`  
		Last Modified: Fri, 20 Nov 2020 13:21:30 GMT  
		Size: 26.7 MB (26708056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf8fb62ba5ffb221a2edb2208741346eb4d2d99a174138e4afbb69ce1fd9966`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 850.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80c964ece6a3edf0db1cfc72ae0e6f0699fb776bbfcc92b708fbb945b0b9547`  
		Last Modified: Wed, 25 Nov 2020 22:26:30 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbdc1b81f30dbbd36bce786a7db45a7e80384faea0379723165445aab33d793`  
		Last Modified: Wed, 25 Nov 2020 23:15:46 GMT  
		Size: 3.0 MB (2975364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d13de64a7cae4a9585b661df831eff6edd11908e8d35b2295637d9cfa318d12`  
		Last Modified: Wed, 25 Nov 2020 23:16:14 GMT  
		Size: 63.5 MB (63491690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; 386

```console
$ docker pull ibmjava@sha256:b3313f5fbb09faf3df5b2ac87e0713b9080a7120e90aa49633273beb00e5ed35
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93053181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:100318974eb9c77e277992f95fe60baa0e4ae9b6db8062e2914b78cc605f6d66`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Nov 2020 22:39:43 GMT
ADD file:0c5561447fe076ca64e04bad6a202d27c7f34e112c49a4f1d6c019f69df4018d in / 
# Wed, 25 Nov 2020 22:39:44 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:39:44 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:39:45 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:39:45 GMT
CMD ["/bin/bash"]
# Wed, 25 Nov 2020 22:56:00 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 25 Nov 2020 22:56:11 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 25 Nov 2020 22:56:11 GMT
ENV JAVA_VERSION=1.8.0_sr6fp16
# Wed, 25 Nov 2020 22:57:40 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d143836caa7e7777f6bf4539b249c48341da97ca4d27f012cf5541b35376e479';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='104b7d07afb812acf1d37a1409cf9dbf360745f346a50a3954ae465315966ad5';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='d2d5ca9484d0801816a74b66551a07d5f69fb41e52aeb5f10ddf1d55c1a46d06';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='dd5d853e9dbbcd7342c7dfb0259b675b951ae1faadbbb667f6553270ceb5b4f8';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='a4b617ba4614317f92159a6930a7ae369923b909377a4d0f2aff9ce3b098ac39';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 25 Nov 2020 22:57:40 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:73fd230d9c9346a670d4a2eca6e4352405d1bfcfeb6039b4018158cde52d0767`  
		Last Modified: Mon, 23 Nov 2020 17:14:15 GMT  
		Size: 27.1 MB (27135125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354328fbe40a654d4fff7b284bbe510445e5c0722de56b7c28dccd50c0b7acf5`  
		Last Modified: Wed, 25 Nov 2020 22:40:15 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100b74721cd5ea3ed3868db1c4835480d2f5332ea99fc6ade8f74b448ec551ac`  
		Last Modified: Wed, 25 Nov 2020 22:40:16 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b27efed6e3036e6bb536fc15474c5c0d57768dfdcbd2a2e8cd670b3e517abb`  
		Last Modified: Wed, 25 Nov 2020 22:58:56 GMT  
		Size: 3.0 MB (3001762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd5a0ec5490fe626ff95181159e1c8cc36f9011f9f4ca11998c489d00d8a326`  
		Last Modified: Wed, 25 Nov 2020 22:59:25 GMT  
		Size: 62.9 MB (62915283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:6c7ab789c56f4bd8a946a3da507c44ae76560bb496b0d3efd97e522ed8f4d801
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.2 MB (97192753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e35ebd6e91e25a825dd97582d10edefba25d79e9a9d853478334acfa9002a05b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 25 Sep 2020 23:47:27 GMT
ADD file:0275f43eb5902c3fb3fe4f7e8dbd20c02f6be138627bbc6770bb74283f9e35fa in / 
# Fri, 25 Sep 2020 23:47:54 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 25 Sep 2020 23:48:12 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 25 Sep 2020 23:48:29 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 25 Sep 2020 23:48:35 GMT
CMD ["/bin/bash"]
# Sat, 26 Sep 2020 04:38:06 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Sat, 26 Sep 2020 04:38:59 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Wed, 30 Sep 2020 00:21:11 GMT
ENV JAVA_VERSION=1.8.0_sr6fp16
# Wed, 30 Sep 2020 00:24:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d143836caa7e7777f6bf4539b249c48341da97ca4d27f012cf5541b35376e479';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='104b7d07afb812acf1d37a1409cf9dbf360745f346a50a3954ae465315966ad5';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='d2d5ca9484d0801816a74b66551a07d5f69fb41e52aeb5f10ddf1d55c1a46d06';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='dd5d853e9dbbcd7342c7dfb0259b675b951ae1faadbbb667f6553270ceb5b4f8';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='a4b617ba4614317f92159a6930a7ae369923b909377a4d0f2aff9ce3b098ac39';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Wed, 30 Sep 2020 00:24:51 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:597e66b6a06b9db7e6c7b74196c96587c89c928a0f1bea6a5c816ed0364acca2`  
		Last Modified: Sat, 26 Sep 2020 00:05:59 GMT  
		Size: 30.4 MB (30408489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe1993d655960561e2b7d98a72bf4167cb6bb3a934b1095c2bd170bce1b0d0`  
		Last Modified: Sat, 26 Sep 2020 00:05:07 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a85181f68a0b81866e1ec4d1fc2f161d8d57137447d2ff1d6d61bcac1974773`  
		Last Modified: Sat, 26 Sep 2020 00:05:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6405e3c1dd428ca3ff035da6469a7c6c36d02c92adb80d285656f61f8dd866b1`  
		Last Modified: Sat, 26 Sep 2020 04:43:33 GMT  
		Size: 3.1 MB (3075371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e21eb6a02583a941df3dec0c0a89fcc197557832a5ad9f0990a6209ed57696`  
		Last Modified: Wed, 30 Sep 2020 00:30:25 GMT  
		Size: 63.7 MB (63707849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; s390x

```console
$ docker pull ibmjava@sha256:80a1971b3d802b8fe84f90bb0e918e403304e10bd2688922b51b85f812c451ee
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.7 MB (92691914 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:daf8b3511d1c1ac4585c94f17e178bf0e32aacadd83a7646439542b5d6007d13`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Nov 2020 22:44:54 GMT
ADD file:aa0063276274c9f3ba9308c3cdfd911449966c87546f28ceb3122d6fbd995d52 in / 
# Wed, 25 Nov 2020 22:45:00 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Wed, 25 Nov 2020 22:45:02 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Wed, 25 Nov 2020 22:45:04 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Wed, 25 Nov 2020 22:45:04 GMT
CMD ["/bin/bash"]
# Thu, 26 Nov 2020 00:11:24 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 26 Nov 2020 00:11:40 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Thu, 26 Nov 2020 00:11:41 GMT
ENV JAVA_VERSION=1.8.0_sr6fp16
# Thu, 26 Nov 2020 00:13:36 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d143836caa7e7777f6bf4539b249c48341da97ca4d27f012cf5541b35376e479';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='104b7d07afb812acf1d37a1409cf9dbf360745f346a50a3954ae465315966ad5';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='d2d5ca9484d0801816a74b66551a07d5f69fb41e52aeb5f10ddf1d55c1a46d06';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='dd5d853e9dbbcd7342c7dfb0259b675b951ae1faadbbb667f6553270ceb5b4f8';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='a4b617ba4614317f92159a6930a7ae369923b909377a4d0f2aff9ce3b098ac39';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Thu, 26 Nov 2020 00:13:41 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:2269433521a3f2e95508abd4fa29a3de21226eed5a09ad3959a689b066151bca`  
		Last Modified: Mon, 23 Nov 2020 18:41:52 GMT  
		Size: 25.4 MB (25381722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4442687b9aa7dcd6b97d4f9ce9562774788922b94571cd3a7ea85185cd76cbd3`  
		Last Modified: Wed, 25 Nov 2020 22:47:07 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6efa602a92c53f638f3667fa4400f2fdb32c5aaae3d112e33f15a12cb2bb3b`  
		Last Modified: Wed, 25 Nov 2020 22:47:06 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7e8278523fb197f7b6968653f981d6e4a73bd83bde2d7fbd11836379af96d3`  
		Last Modified: Thu, 26 Nov 2020 00:15:37 GMT  
		Size: 2.7 MB (2689291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:633a8c71e8db5b9d2f9e55e479ba0f1c348f195c1d982b18e688a27263d9ecb4`  
		Last Modified: Thu, 26 Nov 2020 00:16:04 GMT  
		Size: 64.6 MB (64619862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
