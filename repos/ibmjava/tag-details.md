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
$ docker pull ibmjava@sha256:858c7c1e2991d01447f8dba879d318d5a6dd2c675a01aa8201abc74acb5482f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8` - linux; amd64

```console
$ docker pull ibmjava@sha256:a17d4da78a3e27a1331097be425a7ce38a126956d170a727610e7453c6581e91
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.0 MB (160000703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ee74812172b352e80201b5a2adfaa74ba7b948d4056af4dc275a578562aaa1d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:17:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 23:18:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:18:02 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 23:18:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1203517876025e70b1c66491094cc6ea22704fd56a11f74043611ae5757a5180';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f216652dcc50778d13913dda73ea4b0f423fc0c6c45766fabac2e6f8b51d4b06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a44cddca5e072f3009e852344ce7e01755b87b60ae5cbb03232472db7c27536f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='654052eb2b2e8d95cceb443ac9863b5a038ebd29899b2b6e17825e9d0625b863';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='42345ba0e03b475e2e96336e5479ff94aed4a438002b193f3d3c4dff756c6b2c';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 23:18:45 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260c1687832ae34d925389a567f4eba8837fc1aa6be3f5f417b7342811950856`  
		Last Modified: Fri, 21 Feb 2020 23:20:53 GMT  
		Size: 3.0 MB (2965731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c43ddc9f9a1bb63cf7db9cd4e3d45ee11033e7e4afc351f1c7149187d6b474`  
		Last Modified: Fri, 21 Feb 2020 23:21:04 GMT  
		Size: 130.3 MB (130306496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8` - linux; 386

```console
$ docker pull ibmjava@sha256:d9d75f255581fdbf465e7f23c1fc658abfc4fe8174640bed4859f63f2b2f0281
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148898498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05817440a418bd0cd6f53cdeceacda1fb89da5a4f4bf97b02d5a36f769aac84e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:39:03 GMT
ADD file:df203cc2574204629c69613fcea4942faa0f9224ff0c8bacb908b85d73604628 in / 
# Fri, 21 Feb 2020 21:39:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:39:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:39:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:39:06 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 21:55:45 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 21:55:54 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:54 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 21:56:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1203517876025e70b1c66491094cc6ea22704fd56a11f74043611ae5757a5180';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f216652dcc50778d13913dda73ea4b0f423fc0c6c45766fabac2e6f8b51d4b06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a44cddca5e072f3009e852344ce7e01755b87b60ae5cbb03232472db7c27536f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='654052eb2b2e8d95cceb443ac9863b5a038ebd29899b2b6e17825e9d0625b863';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='42345ba0e03b475e2e96336e5479ff94aed4a438002b193f3d3c4dff756c6b2c';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 21:56:37 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:ddc482e6a4fa5e364980052ab9f5d236f29ae9b217ed672b3dba44669f4041de`  
		Last Modified: Fri, 21 Feb 2020 21:39:58 GMT  
		Size: 27.1 MB (27123823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d2b8bf2fa50513ca7c508e44ac1a15c7ec42b1a3369a91380663868309ab46`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 34.6 KB (34625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84c193628e4067b419327ffa1bfef4b73161d9b1e3ce1e4ee83e714fd1d14e8`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271c42d486e4bb18cadbdf885d057c29384a032113047030f7c4bd6253bbf10`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d6ec2d33bfaf511d9237ee4ecaaf9d1f6b9aea99231bf1bdeb23a03997d84e`  
		Last Modified: Fri, 21 Feb 2020 21:58:25 GMT  
		Size: 3.0 MB (2992872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11b317f53bab418ecfc1c0b3b43f99b04d6609ef61b2ef004cd2df7379dc4a7`  
		Last Modified: Fri, 21 Feb 2020 21:58:37 GMT  
		Size: 118.7 MB (118746172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:78da1602bbf3388aacb94bb2a7781cfc70d96afa30aac57af4912db4161cabc7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176836426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0d3e140c834e9e032d86063d1c70053da7b81caea3ee3b9c162d39d59caf3f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:30:07 GMT
ADD file:fee193b50fa8dbda3e9dbec639709a18c062adef5add2fda1c8aa29e5a288d28 in / 
# Fri, 21 Feb 2020 22:30:18 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:30:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:30:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:30:36 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:07:12 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Sat, 22 Feb 2020 00:07:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:07:40 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Sat, 22 Feb 2020 00:08:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1203517876025e70b1c66491094cc6ea22704fd56a11f74043611ae5757a5180';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f216652dcc50778d13913dda73ea4b0f423fc0c6c45766fabac2e6f8b51d4b06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a44cddca5e072f3009e852344ce7e01755b87b60ae5cbb03232472db7c27536f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='654052eb2b2e8d95cceb443ac9863b5a038ebd29899b2b6e17825e9d0625b863';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='42345ba0e03b475e2e96336e5479ff94aed4a438002b193f3d3c4dff756c6b2c';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Sat, 22 Feb 2020 00:08:48 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:cfb81e1a655db6311df167d6e7259257ac1bec8fd6fa9eaef39c0661b1488490`  
		Last Modified: Fri, 21 Feb 2020 22:33:18 GMT  
		Size: 30.4 MB (30401091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a815faea808b955284818fc847eb2d542dc550d92f5974023b34000a33302aed`  
		Last Modified: Fri, 21 Feb 2020 22:33:12 GMT  
		Size: 35.2 KB (35207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e009f42ff24bbe56824bac50e1ba861b157cbf45a60e8e09ff1f4eee816a21a1`  
		Last Modified: Fri, 21 Feb 2020 22:33:11 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9164e4ca1b0934007f85d8baa8c3041d64dcde54ccfa21f38a106d1b876a1c21`  
		Last Modified: Fri, 21 Feb 2020 22:33:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ed5f62ef19e83fce216082c58e34647c04835dc77ff8bc04cabf8bc7eae7a`  
		Last Modified: Sat, 22 Feb 2020 00:11:32 GMT  
		Size: 3.1 MB (3093403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ad5fe977600e79c4e31fb3e778ef7e2612bb13024d5b93242d44f4a527c4cf`  
		Last Modified: Sat, 22 Feb 2020 00:11:50 GMT  
		Size: 143.3 MB (143305686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8` - linux; s390x

```console
$ docker pull ibmjava@sha256:7c3380ba3143f624dc7d912bb6c142a829d3c4d402c4423b051fb4c5d0f6f3a5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155630549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3079d744cd9b63082cd800addd51241d6bcef9d19bac8d35d306f0fb3b49f5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:57:46 GMT
ADD file:7925c9b35ffa1870e7d336ddcdd6c3434715178c7d08ff2ce9796b651302c347 in / 
# Fri, 21 Feb 2020 21:57:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:57:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:57:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:57:53 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:31:02 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 22:31:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:31:16 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 22:32:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1203517876025e70b1c66491094cc6ea22704fd56a11f74043611ae5757a5180';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f216652dcc50778d13913dda73ea4b0f423fc0c6c45766fabac2e6f8b51d4b06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a44cddca5e072f3009e852344ce7e01755b87b60ae5cbb03232472db7c27536f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='654052eb2b2e8d95cceb443ac9863b5a038ebd29899b2b6e17825e9d0625b863';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='42345ba0e03b475e2e96336e5479ff94aed4a438002b193f3d3c4dff756c6b2c';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 22:32:20 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:b84fcb37dc33cf7416e0f1cf1219e16a15ab0d1c3aa4638d362f19c2679451de`  
		Last Modified: Fri, 21 Feb 2020 21:59:09 GMT  
		Size: 25.4 MB (25365672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9594931f903b7b3c4f5cb63196d29d715c50b567c128a5572131c12a25f04139`  
		Last Modified: Fri, 21 Feb 2020 21:59:06 GMT  
		Size: 36.2 KB (36186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66af13675c2330803d61d2198bb4f69c36bb7eed2d2b2bc3660fed8e873dce59`  
		Last Modified: Fri, 21 Feb 2020 21:59:11 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0fb7b2ee5c5bc387374bdd08f53541bdfcf678d9b9f83489c3923af65fed0`  
		Last Modified: Fri, 21 Feb 2020 21:59:21 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9381eb8b0a499263e6b76868e9412c47073e4d805bb897325f5e2de25846c6e7`  
		Last Modified: Fri, 21 Feb 2020 22:34:51 GMT  
		Size: 2.7 MB (2678898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aed53e3f9a4fd2569e95addcf56d9a518e7f39e0c6bfb15338120a65579742c`  
		Last Modified: Fri, 21 Feb 2020 22:35:01 GMT  
		Size: 127.5 MB (127548758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-jre`

```console
$ docker pull ibmjava@sha256:858c7c1e2991d01447f8dba879d318d5a6dd2c675a01aa8201abc74acb5482f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-jre` - linux; amd64

```console
$ docker pull ibmjava@sha256:a17d4da78a3e27a1331097be425a7ce38a126956d170a727610e7453c6581e91
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.0 MB (160000703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ee74812172b352e80201b5a2adfaa74ba7b948d4056af4dc275a578562aaa1d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:17:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 23:18:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:18:02 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 23:18:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1203517876025e70b1c66491094cc6ea22704fd56a11f74043611ae5757a5180';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f216652dcc50778d13913dda73ea4b0f423fc0c6c45766fabac2e6f8b51d4b06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a44cddca5e072f3009e852344ce7e01755b87b60ae5cbb03232472db7c27536f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='654052eb2b2e8d95cceb443ac9863b5a038ebd29899b2b6e17825e9d0625b863';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='42345ba0e03b475e2e96336e5479ff94aed4a438002b193f3d3c4dff756c6b2c';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 23:18:45 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260c1687832ae34d925389a567f4eba8837fc1aa6be3f5f417b7342811950856`  
		Last Modified: Fri, 21 Feb 2020 23:20:53 GMT  
		Size: 3.0 MB (2965731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c43ddc9f9a1bb63cf7db9cd4e3d45ee11033e7e4afc351f1c7149187d6b474`  
		Last Modified: Fri, 21 Feb 2020 23:21:04 GMT  
		Size: 130.3 MB (130306496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-jre` - linux; 386

```console
$ docker pull ibmjava@sha256:d9d75f255581fdbf465e7f23c1fc658abfc4fe8174640bed4859f63f2b2f0281
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148898498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05817440a418bd0cd6f53cdeceacda1fb89da5a4f4bf97b02d5a36f769aac84e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:39:03 GMT
ADD file:df203cc2574204629c69613fcea4942faa0f9224ff0c8bacb908b85d73604628 in / 
# Fri, 21 Feb 2020 21:39:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:39:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:39:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:39:06 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 21:55:45 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 21:55:54 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:54 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 21:56:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1203517876025e70b1c66491094cc6ea22704fd56a11f74043611ae5757a5180';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f216652dcc50778d13913dda73ea4b0f423fc0c6c45766fabac2e6f8b51d4b06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a44cddca5e072f3009e852344ce7e01755b87b60ae5cbb03232472db7c27536f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='654052eb2b2e8d95cceb443ac9863b5a038ebd29899b2b6e17825e9d0625b863';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='42345ba0e03b475e2e96336e5479ff94aed4a438002b193f3d3c4dff756c6b2c';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 21:56:37 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:ddc482e6a4fa5e364980052ab9f5d236f29ae9b217ed672b3dba44669f4041de`  
		Last Modified: Fri, 21 Feb 2020 21:39:58 GMT  
		Size: 27.1 MB (27123823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d2b8bf2fa50513ca7c508e44ac1a15c7ec42b1a3369a91380663868309ab46`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 34.6 KB (34625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84c193628e4067b419327ffa1bfef4b73161d9b1e3ce1e4ee83e714fd1d14e8`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271c42d486e4bb18cadbdf885d057c29384a032113047030f7c4bd6253bbf10`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d6ec2d33bfaf511d9237ee4ecaaf9d1f6b9aea99231bf1bdeb23a03997d84e`  
		Last Modified: Fri, 21 Feb 2020 21:58:25 GMT  
		Size: 3.0 MB (2992872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11b317f53bab418ecfc1c0b3b43f99b04d6609ef61b2ef004cd2df7379dc4a7`  
		Last Modified: Fri, 21 Feb 2020 21:58:37 GMT  
		Size: 118.7 MB (118746172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-jre` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:78da1602bbf3388aacb94bb2a7781cfc70d96afa30aac57af4912db4161cabc7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176836426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0d3e140c834e9e032d86063d1c70053da7b81caea3ee3b9c162d39d59caf3f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:30:07 GMT
ADD file:fee193b50fa8dbda3e9dbec639709a18c062adef5add2fda1c8aa29e5a288d28 in / 
# Fri, 21 Feb 2020 22:30:18 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:30:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:30:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:30:36 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:07:12 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Sat, 22 Feb 2020 00:07:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:07:40 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Sat, 22 Feb 2020 00:08:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1203517876025e70b1c66491094cc6ea22704fd56a11f74043611ae5757a5180';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f216652dcc50778d13913dda73ea4b0f423fc0c6c45766fabac2e6f8b51d4b06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a44cddca5e072f3009e852344ce7e01755b87b60ae5cbb03232472db7c27536f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='654052eb2b2e8d95cceb443ac9863b5a038ebd29899b2b6e17825e9d0625b863';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='42345ba0e03b475e2e96336e5479ff94aed4a438002b193f3d3c4dff756c6b2c';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Sat, 22 Feb 2020 00:08:48 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:cfb81e1a655db6311df167d6e7259257ac1bec8fd6fa9eaef39c0661b1488490`  
		Last Modified: Fri, 21 Feb 2020 22:33:18 GMT  
		Size: 30.4 MB (30401091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a815faea808b955284818fc847eb2d542dc550d92f5974023b34000a33302aed`  
		Last Modified: Fri, 21 Feb 2020 22:33:12 GMT  
		Size: 35.2 KB (35207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e009f42ff24bbe56824bac50e1ba861b157cbf45a60e8e09ff1f4eee816a21a1`  
		Last Modified: Fri, 21 Feb 2020 22:33:11 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9164e4ca1b0934007f85d8baa8c3041d64dcde54ccfa21f38a106d1b876a1c21`  
		Last Modified: Fri, 21 Feb 2020 22:33:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ed5f62ef19e83fce216082c58e34647c04835dc77ff8bc04cabf8bc7eae7a`  
		Last Modified: Sat, 22 Feb 2020 00:11:32 GMT  
		Size: 3.1 MB (3093403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ad5fe977600e79c4e31fb3e778ef7e2612bb13024d5b93242d44f4a527c4cf`  
		Last Modified: Sat, 22 Feb 2020 00:11:50 GMT  
		Size: 143.3 MB (143305686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-jre` - linux; s390x

```console
$ docker pull ibmjava@sha256:7c3380ba3143f624dc7d912bb6c142a829d3c4d402c4423b051fb4c5d0f6f3a5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155630549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3079d744cd9b63082cd800addd51241d6bcef9d19bac8d35d306f0fb3b49f5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:57:46 GMT
ADD file:7925c9b35ffa1870e7d336ddcdd6c3434715178c7d08ff2ce9796b651302c347 in / 
# Fri, 21 Feb 2020 21:57:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:57:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:57:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:57:53 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:31:02 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 22:31:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:31:16 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 22:32:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1203517876025e70b1c66491094cc6ea22704fd56a11f74043611ae5757a5180';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f216652dcc50778d13913dda73ea4b0f423fc0c6c45766fabac2e6f8b51d4b06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a44cddca5e072f3009e852344ce7e01755b87b60ae5cbb03232472db7c27536f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='654052eb2b2e8d95cceb443ac9863b5a038ebd29899b2b6e17825e9d0625b863';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='42345ba0e03b475e2e96336e5479ff94aed4a438002b193f3d3c4dff756c6b2c';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 22:32:20 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:b84fcb37dc33cf7416e0f1cf1219e16a15ab0d1c3aa4638d362f19c2679451de`  
		Last Modified: Fri, 21 Feb 2020 21:59:09 GMT  
		Size: 25.4 MB (25365672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9594931f903b7b3c4f5cb63196d29d715c50b567c128a5572131c12a25f04139`  
		Last Modified: Fri, 21 Feb 2020 21:59:06 GMT  
		Size: 36.2 KB (36186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66af13675c2330803d61d2198bb4f69c36bb7eed2d2b2bc3660fed8e873dce59`  
		Last Modified: Fri, 21 Feb 2020 21:59:11 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0fb7b2ee5c5bc387374bdd08f53541bdfcf678d9b9f83489c3923af65fed0`  
		Last Modified: Fri, 21 Feb 2020 21:59:21 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9381eb8b0a499263e6b76868e9412c47073e4d805bb897325f5e2de25846c6e7`  
		Last Modified: Fri, 21 Feb 2020 22:34:51 GMT  
		Size: 2.7 MB (2678898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aed53e3f9a4fd2569e95addcf56d9a518e7f39e0c6bfb15338120a65579742c`  
		Last Modified: Fri, 21 Feb 2020 22:35:01 GMT  
		Size: 127.5 MB (127548758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-jre-alpine`

```console
$ docker pull ibmjava@sha256:bb6c4e5e37e7e2648c1adfe7ce49af12add50436336434bb1ff7f845c0a38147
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `ibmjava:8-jre-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:2b9b699e3af4654d5748b4f8628e01f081e8b0fdf1598c3ec8966f9d2bebc140
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138631963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a12b7c1b8e8ce5ac2b439fda80d7d5190ee6a1329e19a95bb9e334d13a03131b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 18:58:11 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 23 Jan 2020 18:58:11 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Thu, 23 Jan 2020 18:58:26 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Wed, 05 Feb 2020 02:15:32 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Wed, 05 Feb 2020 02:16:16 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1203517876025e70b1c66491094cc6ea22704fd56a11f74043611ae5757a5180';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f216652dcc50778d13913dda73ea4b0f423fc0c6c45766fabac2e6f8b51d4b06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a44cddca5e072f3009e852344ce7e01755b87b60ae5cbb03232472db7c27536f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='654052eb2b2e8d95cceb443ac9863b5a038ebd29899b2b6e17825e9d0625b863';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='42345ba0e03b475e2e96336e5479ff94aed4a438002b193f3d3c4dff756c6b2c';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Wed, 05 Feb 2020 02:16:17 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56dae0f47127209aea70646977ebe366124ed65f82542cf651f109356bff110b`  
		Last Modified: Thu, 23 Jan 2020 19:01:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fad1ca64c34cb5644888bf2c8ae8fee9a4b1c9437b10bf8c0242dc13ce232a`  
		Last Modified: Thu, 23 Jan 2020 19:01:33 GMT  
		Size: 5.6 MB (5565608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1e41e75f16d77a5f5ddf7f49969ae2d3897e5876a9ec18676b15b71d9b03d7`  
		Last Modified: Wed, 05 Feb 2020 02:22:00 GMT  
		Size: 130.3 MB (130278848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-sdk`

```console
$ docker pull ibmjava@sha256:e0b58c30610556cb0908fcf1881aabdd67642a10c209286723ba5944e629faf0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-sdk` - linux; amd64

```console
$ docker pull ibmjava@sha256:f6d1d9274601046eaef66bd217ad2ffb963c5f203af2bd8effbf331e7f3f5a59
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.2 MB (197164339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4083a7df6c6e099c1f3d01cf3ba89066c914712845cc94cbaa58405752cee5ad`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:17:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 23:18:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:18:02 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 23:20:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='a640a2fbdb3cef7faa68f9349060ca5f7ce403ca351c599f6bdd28ba0b9cfd8b';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='198a58f224d5d186c18f892e2372a8224fd20de876bf407a33b14e1992d6e1ff';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='16a0104383e0c3a1bcef066b15518ea1fdc91d630113297617b7c1a5a786f08b';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='deb2a801e04199711d66c2407c81c39b706afebe4eb6b5db864e8228c9f887c4';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='f70cb53a51e32fcbc6ccf367fbb7d23330fbf19d3c49e079efceb10403c7b470';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 23:20:32 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260c1687832ae34d925389a567f4eba8837fc1aa6be3f5f417b7342811950856`  
		Last Modified: Fri, 21 Feb 2020 23:20:53 GMT  
		Size: 3.0 MB (2965731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a73079cba01de6bce06aaa395d4f2de238d0241f3bb5e5d51bb23b0f4ae5a`  
		Last Modified: Fri, 21 Feb 2020 23:21:35 GMT  
		Size: 167.5 MB (167470132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; 386

```console
$ docker pull ibmjava@sha256:b70afef2aaeba2c1234e49be4e6461fdf47e27839e95c85dde035dc120d525fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.0 MB (185957610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a52513788feb213292ade8b467e187d22646e43a8ce230be0581cd7081b3d84d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:39:03 GMT
ADD file:df203cc2574204629c69613fcea4942faa0f9224ff0c8bacb908b85d73604628 in / 
# Fri, 21 Feb 2020 21:39:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:39:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:39:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:39:06 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 21:55:45 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 21:55:54 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:54 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 21:58:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='a640a2fbdb3cef7faa68f9349060ca5f7ce403ca351c599f6bdd28ba0b9cfd8b';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='198a58f224d5d186c18f892e2372a8224fd20de876bf407a33b14e1992d6e1ff';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='16a0104383e0c3a1bcef066b15518ea1fdc91d630113297617b7c1a5a786f08b';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='deb2a801e04199711d66c2407c81c39b706afebe4eb6b5db864e8228c9f887c4';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='f70cb53a51e32fcbc6ccf367fbb7d23330fbf19d3c49e079efceb10403c7b470';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 21:58:17 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:ddc482e6a4fa5e364980052ab9f5d236f29ae9b217ed672b3dba44669f4041de`  
		Last Modified: Fri, 21 Feb 2020 21:39:58 GMT  
		Size: 27.1 MB (27123823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d2b8bf2fa50513ca7c508e44ac1a15c7ec42b1a3369a91380663868309ab46`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 34.6 KB (34625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84c193628e4067b419327ffa1bfef4b73161d9b1e3ce1e4ee83e714fd1d14e8`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271c42d486e4bb18cadbdf885d057c29384a032113047030f7c4bd6253bbf10`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d6ec2d33bfaf511d9237ee4ecaaf9d1f6b9aea99231bf1bdeb23a03997d84e`  
		Last Modified: Fri, 21 Feb 2020 21:58:25 GMT  
		Size: 3.0 MB (2992872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e13f152e74d140854578805c947c6351b0025a2cfd89c5f3be22b584b4e545`  
		Last Modified: Fri, 21 Feb 2020 21:59:10 GMT  
		Size: 155.8 MB (155805284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:aaa45d323bb6551c7758ce7bd3049a60998851c57cf7ff5dede134001f64e627
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.1 MB (214118404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76aea1f3d48c97cbc3e845a9125b3d35a73c90df8f1d68cc272e97aa30f97ff3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:30:07 GMT
ADD file:fee193b50fa8dbda3e9dbec639709a18c062adef5add2fda1c8aa29e5a288d28 in / 
# Fri, 21 Feb 2020 22:30:18 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:30:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:30:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:30:36 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:07:12 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Sat, 22 Feb 2020 00:07:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:07:40 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Sat, 22 Feb 2020 00:11:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='a640a2fbdb3cef7faa68f9349060ca5f7ce403ca351c599f6bdd28ba0b9cfd8b';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='198a58f224d5d186c18f892e2372a8224fd20de876bf407a33b14e1992d6e1ff';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='16a0104383e0c3a1bcef066b15518ea1fdc91d630113297617b7c1a5a786f08b';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='deb2a801e04199711d66c2407c81c39b706afebe4eb6b5db864e8228c9f887c4';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='f70cb53a51e32fcbc6ccf367fbb7d23330fbf19d3c49e079efceb10403c7b470';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Sat, 22 Feb 2020 00:11:13 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:cfb81e1a655db6311df167d6e7259257ac1bec8fd6fa9eaef39c0661b1488490`  
		Last Modified: Fri, 21 Feb 2020 22:33:18 GMT  
		Size: 30.4 MB (30401091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a815faea808b955284818fc847eb2d542dc550d92f5974023b34000a33302aed`  
		Last Modified: Fri, 21 Feb 2020 22:33:12 GMT  
		Size: 35.2 KB (35207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e009f42ff24bbe56824bac50e1ba861b157cbf45a60e8e09ff1f4eee816a21a1`  
		Last Modified: Fri, 21 Feb 2020 22:33:11 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9164e4ca1b0934007f85d8baa8c3041d64dcde54ccfa21f38a106d1b876a1c21`  
		Last Modified: Fri, 21 Feb 2020 22:33:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ed5f62ef19e83fce216082c58e34647c04835dc77ff8bc04cabf8bc7eae7a`  
		Last Modified: Sat, 22 Feb 2020 00:11:32 GMT  
		Size: 3.1 MB (3093403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843d7c458af99a59c62f2e575db2982d334ad826bab5831bd1f814c942c71036`  
		Last Modified: Sat, 22 Feb 2020 00:12:47 GMT  
		Size: 180.6 MB (180587664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sdk` - linux; s390x

```console
$ docker pull ibmjava@sha256:0c5253c25629a7a767f58924384bff8548ed6cd909a087478633cf22d46f6b54
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.9 MB (185874896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adecfc855c63d3fd990bd40016886d53f102a0ebce14d4a1fd102de84b06f9af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:57:46 GMT
ADD file:7925c9b35ffa1870e7d336ddcdd6c3434715178c7d08ff2ce9796b651302c347 in / 
# Fri, 21 Feb 2020 21:57:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:57:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:57:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:57:53 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:31:02 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 22:31:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:31:16 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 22:34:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='a640a2fbdb3cef7faa68f9349060ca5f7ce403ca351c599f6bdd28ba0b9cfd8b';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='198a58f224d5d186c18f892e2372a8224fd20de876bf407a33b14e1992d6e1ff';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='16a0104383e0c3a1bcef066b15518ea1fdc91d630113297617b7c1a5a786f08b';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='deb2a801e04199711d66c2407c81c39b706afebe4eb6b5db864e8228c9f887c4';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='f70cb53a51e32fcbc6ccf367fbb7d23330fbf19d3c49e079efceb10403c7b470';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 22:34:38 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:b84fcb37dc33cf7416e0f1cf1219e16a15ab0d1c3aa4638d362f19c2679451de`  
		Last Modified: Fri, 21 Feb 2020 21:59:09 GMT  
		Size: 25.4 MB (25365672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9594931f903b7b3c4f5cb63196d29d715c50b567c128a5572131c12a25f04139`  
		Last Modified: Fri, 21 Feb 2020 21:59:06 GMT  
		Size: 36.2 KB (36186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66af13675c2330803d61d2198bb4f69c36bb7eed2d2b2bc3660fed8e873dce59`  
		Last Modified: Fri, 21 Feb 2020 21:59:11 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0fb7b2ee5c5bc387374bdd08f53541bdfcf678d9b9f83489c3923af65fed0`  
		Last Modified: Fri, 21 Feb 2020 21:59:21 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9381eb8b0a499263e6b76868e9412c47073e4d805bb897325f5e2de25846c6e7`  
		Last Modified: Fri, 21 Feb 2020 22:34:51 GMT  
		Size: 2.7 MB (2678898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188efe0c77413e1999ba1841b1b05ad7b5d34078c243847f9f2b1fe96f2cf66b`  
		Last Modified: Fri, 21 Feb 2020 22:35:34 GMT  
		Size: 157.8 MB (157793105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-sdk-alpine`

```console
$ docker pull ibmjava@sha256:f0cb037c1f3f2558743a8bcc96dcc995ed6c0f11532ef6265bbe7541a18b79f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `ibmjava:8-sdk-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:fc0783d65ae3c76f70acbc452036ecc12d44fd4efbba5bb4c55a1b7d294471b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.8 MB (175794023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:985a0bb7027890015088cfa7019fc3294f2f92ce21bdf5cbdb0bd8d2301da1f3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 18:58:11 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 23 Jan 2020 18:58:11 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Thu, 23 Jan 2020 18:58:26 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Wed, 05 Feb 2020 02:15:32 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Wed, 05 Feb 2020 02:19:59 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='a640a2fbdb3cef7faa68f9349060ca5f7ce403ca351c599f6bdd28ba0b9cfd8b';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='198a58f224d5d186c18f892e2372a8224fd20de876bf407a33b14e1992d6e1ff';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='16a0104383e0c3a1bcef066b15518ea1fdc91d630113297617b7c1a5a786f08b';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='deb2a801e04199711d66c2407c81c39b706afebe4eb6b5db864e8228c9f887c4';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='f70cb53a51e32fcbc6ccf367fbb7d23330fbf19d3c49e079efceb10403c7b470';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Wed, 05 Feb 2020 02:19:59 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56dae0f47127209aea70646977ebe366124ed65f82542cf651f109356bff110b`  
		Last Modified: Thu, 23 Jan 2020 19:01:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fad1ca64c34cb5644888bf2c8ae8fee9a4b1c9437b10bf8c0242dc13ce232a`  
		Last Modified: Thu, 23 Jan 2020 19:01:33 GMT  
		Size: 5.6 MB (5565608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caa3d42c822b52e4a611f05d8ab9025fc59ce84b59e8d348f9e5071ea1d8d84`  
		Last Modified: Wed, 05 Feb 2020 02:25:32 GMT  
		Size: 167.4 MB (167440908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-sfj`

```console
$ docker pull ibmjava@sha256:2245db2f61875d55c4bf80e4d67651d0ee2e50cca9e67521475b48a4dbf93eb6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-sfj` - linux; amd64

```console
$ docker pull ibmjava@sha256:ca22e7111199088e1a47bbba293a778d6ef2be8d2cfb2b38dc58908b409a762c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93244430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01e2f4d1bc75ac6e4da33b1a1fb5b51d9b69232c3d8b2bdf6c08d3247f7effaa`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:17:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 23:18:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:18:02 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 23:19:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bf7a6a9901ffab156683981546e75574f987973e03e839bb7249b918e314c4d8';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='d5982516f4e06468956ab89e084843c01ef08c3ed8e40378d33ebb586c92e9ce';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='c7d5cd7aa38879f88eda3e15ab6c1e76a5523522952b143cc2e9d971ef7876ed';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='a1ada0e17749fc87e187654e4b5a985c804397c00e4c3754494ec558d34ff738';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='429b0046251ca3c8ea663ee7fca4e07e35cbefb681977471e4bf5082590be160';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 23:19:32 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260c1687832ae34d925389a567f4eba8837fc1aa6be3f5f417b7342811950856`  
		Last Modified: Fri, 21 Feb 2020 23:20:53 GMT  
		Size: 3.0 MB (2965731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a126cb7083d1eb53cc33b598084bdd4fec0c70d02553f6b33b97cf5399a3d996`  
		Last Modified: Fri, 21 Feb 2020 23:21:17 GMT  
		Size: 63.6 MB (63550223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; 386

```console
$ docker pull ibmjava@sha256:55279810cd6b7d49e3f831d6fb8dafeefec19d47861bc549eaf1892823c87fea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93126563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ac2f0b5e68ec69f1cc6e16c936eadaa2d348810a7c000e8969824498e6a21ee`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:39:03 GMT
ADD file:df203cc2574204629c69613fcea4942faa0f9224ff0c8bacb908b85d73604628 in / 
# Fri, 21 Feb 2020 21:39:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:39:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:39:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:39:06 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 21:55:45 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 21:55:54 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:54 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 21:57:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bf7a6a9901ffab156683981546e75574f987973e03e839bb7249b918e314c4d8';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='d5982516f4e06468956ab89e084843c01ef08c3ed8e40378d33ebb586c92e9ce';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='c7d5cd7aa38879f88eda3e15ab6c1e76a5523522952b143cc2e9d971ef7876ed';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='a1ada0e17749fc87e187654e4b5a985c804397c00e4c3754494ec558d34ff738';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='429b0046251ca3c8ea663ee7fca4e07e35cbefb681977471e4bf5082590be160';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 21:57:21 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:ddc482e6a4fa5e364980052ab9f5d236f29ae9b217ed672b3dba44669f4041de`  
		Last Modified: Fri, 21 Feb 2020 21:39:58 GMT  
		Size: 27.1 MB (27123823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d2b8bf2fa50513ca7c508e44ac1a15c7ec42b1a3369a91380663868309ab46`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 34.6 KB (34625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84c193628e4067b419327ffa1bfef4b73161d9b1e3ce1e4ee83e714fd1d14e8`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271c42d486e4bb18cadbdf885d057c29384a032113047030f7c4bd6253bbf10`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d6ec2d33bfaf511d9237ee4ecaaf9d1f6b9aea99231bf1bdeb23a03997d84e`  
		Last Modified: Fri, 21 Feb 2020 21:58:25 GMT  
		Size: 3.0 MB (2992872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3dd9a327e0abdb50631718508cb757e3929071d01a5340b2dfffa112bfc12d`  
		Last Modified: Fri, 21 Feb 2020 21:58:50 GMT  
		Size: 63.0 MB (62974237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:a82328b940a81f4f66b2578fb289ddcab849b18db2d38dd331d7cb710c0c63d4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.7 MB (101696182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8216295d9cb9a9f807e939f49b2c988458cf287d7bfca6fa5eaacad4f32f475`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:30:07 GMT
ADD file:fee193b50fa8dbda3e9dbec639709a18c062adef5add2fda1c8aa29e5a288d28 in / 
# Fri, 21 Feb 2020 22:30:18 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:30:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:30:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:30:36 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:07:12 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Sat, 22 Feb 2020 00:07:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:07:40 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Sat, 22 Feb 2020 00:09:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bf7a6a9901ffab156683981546e75574f987973e03e839bb7249b918e314c4d8';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='d5982516f4e06468956ab89e084843c01ef08c3ed8e40378d33ebb586c92e9ce';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='c7d5cd7aa38879f88eda3e15ab6c1e76a5523522952b143cc2e9d971ef7876ed';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='a1ada0e17749fc87e187654e4b5a985c804397c00e4c3754494ec558d34ff738';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='429b0046251ca3c8ea663ee7fca4e07e35cbefb681977471e4bf5082590be160';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Sat, 22 Feb 2020 00:09:45 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:cfb81e1a655db6311df167d6e7259257ac1bec8fd6fa9eaef39c0661b1488490`  
		Last Modified: Fri, 21 Feb 2020 22:33:18 GMT  
		Size: 30.4 MB (30401091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a815faea808b955284818fc847eb2d542dc550d92f5974023b34000a33302aed`  
		Last Modified: Fri, 21 Feb 2020 22:33:12 GMT  
		Size: 35.2 KB (35207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e009f42ff24bbe56824bac50e1ba861b157cbf45a60e8e09ff1f4eee816a21a1`  
		Last Modified: Fri, 21 Feb 2020 22:33:11 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9164e4ca1b0934007f85d8baa8c3041d64dcde54ccfa21f38a106d1b876a1c21`  
		Last Modified: Fri, 21 Feb 2020 22:33:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ed5f62ef19e83fce216082c58e34647c04835dc77ff8bc04cabf8bc7eae7a`  
		Last Modified: Sat, 22 Feb 2020 00:11:32 GMT  
		Size: 3.1 MB (3093403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe9d4dfbb66823b78577dbae336c3673f800ffd00cb33cb78590fdaa78d18ec`  
		Last Modified: Sat, 22 Feb 2020 00:12:15 GMT  
		Size: 68.2 MB (68165442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; s390x

```console
$ docker pull ibmjava@sha256:cdfb5b3803e8b2845f1dd1e0bb5a1d8e4861055514102945c332f1c014ca337e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.8 MB (92771969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c2f9c953d8d00a6e47802d9196805c2f8036b55d231804df5250a201fd2ecc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:57:46 GMT
ADD file:7925c9b35ffa1870e7d336ddcdd6c3434715178c7d08ff2ce9796b651302c347 in / 
# Fri, 21 Feb 2020 21:57:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:57:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:57:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:57:53 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:31:02 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 22:31:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:31:16 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 22:33:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bf7a6a9901ffab156683981546e75574f987973e03e839bb7249b918e314c4d8';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='d5982516f4e06468956ab89e084843c01ef08c3ed8e40378d33ebb586c92e9ce';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='c7d5cd7aa38879f88eda3e15ab6c1e76a5523522952b143cc2e9d971ef7876ed';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='a1ada0e17749fc87e187654e4b5a985c804397c00e4c3754494ec558d34ff738';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='429b0046251ca3c8ea663ee7fca4e07e35cbefb681977471e4bf5082590be160';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 22:33:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:b84fcb37dc33cf7416e0f1cf1219e16a15ab0d1c3aa4638d362f19c2679451de`  
		Last Modified: Fri, 21 Feb 2020 21:59:09 GMT  
		Size: 25.4 MB (25365672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9594931f903b7b3c4f5cb63196d29d715c50b567c128a5572131c12a25f04139`  
		Last Modified: Fri, 21 Feb 2020 21:59:06 GMT  
		Size: 36.2 KB (36186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66af13675c2330803d61d2198bb4f69c36bb7eed2d2b2bc3660fed8e873dce59`  
		Last Modified: Fri, 21 Feb 2020 21:59:11 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0fb7b2ee5c5bc387374bdd08f53541bdfcf678d9b9f83489c3923af65fed0`  
		Last Modified: Fri, 21 Feb 2020 21:59:21 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9381eb8b0a499263e6b76868e9412c47073e4d805bb897325f5e2de25846c6e7`  
		Last Modified: Fri, 21 Feb 2020 22:34:51 GMT  
		Size: 2.7 MB (2678898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b471e3d97141df2f163d47de2e6222ce235a9476a72075db044277ae28c96f`  
		Last Modified: Fri, 21 Feb 2020 22:35:16 GMT  
		Size: 64.7 MB (64690178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:8-sfj-alpine`

```console
$ docker pull ibmjava@sha256:b00fffba2515014190e8ebb35535d2a19aecb531f53cb1235cf7b46543255a3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `ibmjava:8-sfj-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:21b66e7c20f804fc75e02c0b6d36f8ca3a89a9c30d5ea6ddf527c631d2a739cb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71917320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b289517bb3624bc26e9bcf388d2aa366c351bdc2600ed8b739944e5fbe55cc66`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 18:58:11 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 23 Jan 2020 18:58:11 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Thu, 23 Jan 2020 18:58:26 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Wed, 05 Feb 2020 02:15:32 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Wed, 05 Feb 2020 02:17:44 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bf7a6a9901ffab156683981546e75574f987973e03e839bb7249b918e314c4d8';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='d5982516f4e06468956ab89e084843c01ef08c3ed8e40378d33ebb586c92e9ce';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='c7d5cd7aa38879f88eda3e15ab6c1e76a5523522952b143cc2e9d971ef7876ed';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='a1ada0e17749fc87e187654e4b5a985c804397c00e4c3754494ec558d34ff738';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='429b0046251ca3c8ea663ee7fca4e07e35cbefb681977471e4bf5082590be160';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Wed, 05 Feb 2020 02:17:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56dae0f47127209aea70646977ebe366124ed65f82542cf651f109356bff110b`  
		Last Modified: Thu, 23 Jan 2020 19:01:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fad1ca64c34cb5644888bf2c8ae8fee9a4b1c9437b10bf8c0242dc13ce232a`  
		Last Modified: Thu, 23 Jan 2020 19:01:33 GMT  
		Size: 5.6 MB (5565608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2e2c0a8d924df9316c50e4bc8eab430b8c2c6057ac72d2ca006ca712403d3f`  
		Last Modified: Wed, 05 Feb 2020 02:22:28 GMT  
		Size: 63.6 MB (63564205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:jre`

```console
$ docker pull ibmjava@sha256:858c7c1e2991d01447f8dba879d318d5a6dd2c675a01aa8201abc74acb5482f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:jre` - linux; amd64

```console
$ docker pull ibmjava@sha256:a17d4da78a3e27a1331097be425a7ce38a126956d170a727610e7453c6581e91
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.0 MB (160000703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ee74812172b352e80201b5a2adfaa74ba7b948d4056af4dc275a578562aaa1d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:17:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 23:18:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:18:02 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 23:18:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1203517876025e70b1c66491094cc6ea22704fd56a11f74043611ae5757a5180';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f216652dcc50778d13913dda73ea4b0f423fc0c6c45766fabac2e6f8b51d4b06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a44cddca5e072f3009e852344ce7e01755b87b60ae5cbb03232472db7c27536f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='654052eb2b2e8d95cceb443ac9863b5a038ebd29899b2b6e17825e9d0625b863';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='42345ba0e03b475e2e96336e5479ff94aed4a438002b193f3d3c4dff756c6b2c';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 23:18:45 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260c1687832ae34d925389a567f4eba8837fc1aa6be3f5f417b7342811950856`  
		Last Modified: Fri, 21 Feb 2020 23:20:53 GMT  
		Size: 3.0 MB (2965731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c43ddc9f9a1bb63cf7db9cd4e3d45ee11033e7e4afc351f1c7149187d6b474`  
		Last Modified: Fri, 21 Feb 2020 23:21:04 GMT  
		Size: 130.3 MB (130306496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:jre` - linux; 386

```console
$ docker pull ibmjava@sha256:d9d75f255581fdbf465e7f23c1fc658abfc4fe8174640bed4859f63f2b2f0281
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148898498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05817440a418bd0cd6f53cdeceacda1fb89da5a4f4bf97b02d5a36f769aac84e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:39:03 GMT
ADD file:df203cc2574204629c69613fcea4942faa0f9224ff0c8bacb908b85d73604628 in / 
# Fri, 21 Feb 2020 21:39:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:39:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:39:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:39:06 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 21:55:45 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 21:55:54 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:54 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 21:56:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1203517876025e70b1c66491094cc6ea22704fd56a11f74043611ae5757a5180';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f216652dcc50778d13913dda73ea4b0f423fc0c6c45766fabac2e6f8b51d4b06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a44cddca5e072f3009e852344ce7e01755b87b60ae5cbb03232472db7c27536f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='654052eb2b2e8d95cceb443ac9863b5a038ebd29899b2b6e17825e9d0625b863';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='42345ba0e03b475e2e96336e5479ff94aed4a438002b193f3d3c4dff756c6b2c';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 21:56:37 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:ddc482e6a4fa5e364980052ab9f5d236f29ae9b217ed672b3dba44669f4041de`  
		Last Modified: Fri, 21 Feb 2020 21:39:58 GMT  
		Size: 27.1 MB (27123823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d2b8bf2fa50513ca7c508e44ac1a15c7ec42b1a3369a91380663868309ab46`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 34.6 KB (34625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84c193628e4067b419327ffa1bfef4b73161d9b1e3ce1e4ee83e714fd1d14e8`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271c42d486e4bb18cadbdf885d057c29384a032113047030f7c4bd6253bbf10`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d6ec2d33bfaf511d9237ee4ecaaf9d1f6b9aea99231bf1bdeb23a03997d84e`  
		Last Modified: Fri, 21 Feb 2020 21:58:25 GMT  
		Size: 3.0 MB (2992872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11b317f53bab418ecfc1c0b3b43f99b04d6609ef61b2ef004cd2df7379dc4a7`  
		Last Modified: Fri, 21 Feb 2020 21:58:37 GMT  
		Size: 118.7 MB (118746172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:jre` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:78da1602bbf3388aacb94bb2a7781cfc70d96afa30aac57af4912db4161cabc7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176836426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0d3e140c834e9e032d86063d1c70053da7b81caea3ee3b9c162d39d59caf3f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:30:07 GMT
ADD file:fee193b50fa8dbda3e9dbec639709a18c062adef5add2fda1c8aa29e5a288d28 in / 
# Fri, 21 Feb 2020 22:30:18 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:30:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:30:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:30:36 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:07:12 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Sat, 22 Feb 2020 00:07:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:07:40 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Sat, 22 Feb 2020 00:08:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1203517876025e70b1c66491094cc6ea22704fd56a11f74043611ae5757a5180';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f216652dcc50778d13913dda73ea4b0f423fc0c6c45766fabac2e6f8b51d4b06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a44cddca5e072f3009e852344ce7e01755b87b60ae5cbb03232472db7c27536f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='654052eb2b2e8d95cceb443ac9863b5a038ebd29899b2b6e17825e9d0625b863';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='42345ba0e03b475e2e96336e5479ff94aed4a438002b193f3d3c4dff756c6b2c';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Sat, 22 Feb 2020 00:08:48 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:cfb81e1a655db6311df167d6e7259257ac1bec8fd6fa9eaef39c0661b1488490`  
		Last Modified: Fri, 21 Feb 2020 22:33:18 GMT  
		Size: 30.4 MB (30401091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a815faea808b955284818fc847eb2d542dc550d92f5974023b34000a33302aed`  
		Last Modified: Fri, 21 Feb 2020 22:33:12 GMT  
		Size: 35.2 KB (35207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e009f42ff24bbe56824bac50e1ba861b157cbf45a60e8e09ff1f4eee816a21a1`  
		Last Modified: Fri, 21 Feb 2020 22:33:11 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9164e4ca1b0934007f85d8baa8c3041d64dcde54ccfa21f38a106d1b876a1c21`  
		Last Modified: Fri, 21 Feb 2020 22:33:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ed5f62ef19e83fce216082c58e34647c04835dc77ff8bc04cabf8bc7eae7a`  
		Last Modified: Sat, 22 Feb 2020 00:11:32 GMT  
		Size: 3.1 MB (3093403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ad5fe977600e79c4e31fb3e778ef7e2612bb13024d5b93242d44f4a527c4cf`  
		Last Modified: Sat, 22 Feb 2020 00:11:50 GMT  
		Size: 143.3 MB (143305686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:jre` - linux; s390x

```console
$ docker pull ibmjava@sha256:7c3380ba3143f624dc7d912bb6c142a829d3c4d402c4423b051fb4c5d0f6f3a5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155630549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3079d744cd9b63082cd800addd51241d6bcef9d19bac8d35d306f0fb3b49f5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:57:46 GMT
ADD file:7925c9b35ffa1870e7d336ddcdd6c3434715178c7d08ff2ce9796b651302c347 in / 
# Fri, 21 Feb 2020 21:57:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:57:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:57:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:57:53 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:31:02 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 22:31:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:31:16 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 22:32:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1203517876025e70b1c66491094cc6ea22704fd56a11f74043611ae5757a5180';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f216652dcc50778d13913dda73ea4b0f423fc0c6c45766fabac2e6f8b51d4b06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a44cddca5e072f3009e852344ce7e01755b87b60ae5cbb03232472db7c27536f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='654052eb2b2e8d95cceb443ac9863b5a038ebd29899b2b6e17825e9d0625b863';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='42345ba0e03b475e2e96336e5479ff94aed4a438002b193f3d3c4dff756c6b2c';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 22:32:20 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:b84fcb37dc33cf7416e0f1cf1219e16a15ab0d1c3aa4638d362f19c2679451de`  
		Last Modified: Fri, 21 Feb 2020 21:59:09 GMT  
		Size: 25.4 MB (25365672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9594931f903b7b3c4f5cb63196d29d715c50b567c128a5572131c12a25f04139`  
		Last Modified: Fri, 21 Feb 2020 21:59:06 GMT  
		Size: 36.2 KB (36186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66af13675c2330803d61d2198bb4f69c36bb7eed2d2b2bc3660fed8e873dce59`  
		Last Modified: Fri, 21 Feb 2020 21:59:11 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0fb7b2ee5c5bc387374bdd08f53541bdfcf678d9b9f83489c3923af65fed0`  
		Last Modified: Fri, 21 Feb 2020 21:59:21 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9381eb8b0a499263e6b76868e9412c47073e4d805bb897325f5e2de25846c6e7`  
		Last Modified: Fri, 21 Feb 2020 22:34:51 GMT  
		Size: 2.7 MB (2678898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aed53e3f9a4fd2569e95addcf56d9a518e7f39e0c6bfb15338120a65579742c`  
		Last Modified: Fri, 21 Feb 2020 22:35:01 GMT  
		Size: 127.5 MB (127548758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:jre-alpine`

```console
$ docker pull ibmjava@sha256:bb6c4e5e37e7e2648c1adfe7ce49af12add50436336434bb1ff7f845c0a38147
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `ibmjava:jre-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:2b9b699e3af4654d5748b4f8628e01f081e8b0fdf1598c3ec8966f9d2bebc140
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.6 MB (138631963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a12b7c1b8e8ce5ac2b439fda80d7d5190ee6a1329e19a95bb9e334d13a03131b`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 18:58:11 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 23 Jan 2020 18:58:11 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Thu, 23 Jan 2020 18:58:26 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Wed, 05 Feb 2020 02:15:32 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Wed, 05 Feb 2020 02:16:16 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1203517876025e70b1c66491094cc6ea22704fd56a11f74043611ae5757a5180';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f216652dcc50778d13913dda73ea4b0f423fc0c6c45766fabac2e6f8b51d4b06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a44cddca5e072f3009e852344ce7e01755b87b60ae5cbb03232472db7c27536f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='654052eb2b2e8d95cceb443ac9863b5a038ebd29899b2b6e17825e9d0625b863';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='42345ba0e03b475e2e96336e5479ff94aed4a438002b193f3d3c4dff756c6b2c';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Wed, 05 Feb 2020 02:16:17 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56dae0f47127209aea70646977ebe366124ed65f82542cf651f109356bff110b`  
		Last Modified: Thu, 23 Jan 2020 19:01:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fad1ca64c34cb5644888bf2c8ae8fee9a4b1c9437b10bf8c0242dc13ce232a`  
		Last Modified: Thu, 23 Jan 2020 19:01:33 GMT  
		Size: 5.6 MB (5565608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1e41e75f16d77a5f5ddf7f49969ae2d3897e5876a9ec18676b15b71d9b03d7`  
		Last Modified: Wed, 05 Feb 2020 02:22:00 GMT  
		Size: 130.3 MB (130278848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:latest`

```console
$ docker pull ibmjava@sha256:858c7c1e2991d01447f8dba879d318d5a6dd2c675a01aa8201abc74acb5482f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:latest` - linux; amd64

```console
$ docker pull ibmjava@sha256:a17d4da78a3e27a1331097be425a7ce38a126956d170a727610e7453c6581e91
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.0 MB (160000703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ee74812172b352e80201b5a2adfaa74ba7b948d4056af4dc275a578562aaa1d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:17:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 23:18:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:18:02 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 23:18:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1203517876025e70b1c66491094cc6ea22704fd56a11f74043611ae5757a5180';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f216652dcc50778d13913dda73ea4b0f423fc0c6c45766fabac2e6f8b51d4b06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a44cddca5e072f3009e852344ce7e01755b87b60ae5cbb03232472db7c27536f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='654052eb2b2e8d95cceb443ac9863b5a038ebd29899b2b6e17825e9d0625b863';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='42345ba0e03b475e2e96336e5479ff94aed4a438002b193f3d3c4dff756c6b2c';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 23:18:45 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260c1687832ae34d925389a567f4eba8837fc1aa6be3f5f417b7342811950856`  
		Last Modified: Fri, 21 Feb 2020 23:20:53 GMT  
		Size: 3.0 MB (2965731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38c43ddc9f9a1bb63cf7db9cd4e3d45ee11033e7e4afc351f1c7149187d6b474`  
		Last Modified: Fri, 21 Feb 2020 23:21:04 GMT  
		Size: 130.3 MB (130306496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:latest` - linux; 386

```console
$ docker pull ibmjava@sha256:d9d75f255581fdbf465e7f23c1fc658abfc4fe8174640bed4859f63f2b2f0281
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.9 MB (148898498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05817440a418bd0cd6f53cdeceacda1fb89da5a4f4bf97b02d5a36f769aac84e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:39:03 GMT
ADD file:df203cc2574204629c69613fcea4942faa0f9224ff0c8bacb908b85d73604628 in / 
# Fri, 21 Feb 2020 21:39:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:39:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:39:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:39:06 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 21:55:45 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 21:55:54 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:54 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 21:56:37 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1203517876025e70b1c66491094cc6ea22704fd56a11f74043611ae5757a5180';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f216652dcc50778d13913dda73ea4b0f423fc0c6c45766fabac2e6f8b51d4b06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a44cddca5e072f3009e852344ce7e01755b87b60ae5cbb03232472db7c27536f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='654052eb2b2e8d95cceb443ac9863b5a038ebd29899b2b6e17825e9d0625b863';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='42345ba0e03b475e2e96336e5479ff94aed4a438002b193f3d3c4dff756c6b2c';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 21:56:37 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:ddc482e6a4fa5e364980052ab9f5d236f29ae9b217ed672b3dba44669f4041de`  
		Last Modified: Fri, 21 Feb 2020 21:39:58 GMT  
		Size: 27.1 MB (27123823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d2b8bf2fa50513ca7c508e44ac1a15c7ec42b1a3369a91380663868309ab46`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 34.6 KB (34625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84c193628e4067b419327ffa1bfef4b73161d9b1e3ce1e4ee83e714fd1d14e8`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271c42d486e4bb18cadbdf885d057c29384a032113047030f7c4bd6253bbf10`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d6ec2d33bfaf511d9237ee4ecaaf9d1f6b9aea99231bf1bdeb23a03997d84e`  
		Last Modified: Fri, 21 Feb 2020 21:58:25 GMT  
		Size: 3.0 MB (2992872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c11b317f53bab418ecfc1c0b3b43f99b04d6609ef61b2ef004cd2df7379dc4a7`  
		Last Modified: Fri, 21 Feb 2020 21:58:37 GMT  
		Size: 118.7 MB (118746172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:latest` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:78da1602bbf3388aacb94bb2a7781cfc70d96afa30aac57af4912db4161cabc7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **176.8 MB (176836426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0d3e140c834e9e032d86063d1c70053da7b81caea3ee3b9c162d39d59caf3f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:30:07 GMT
ADD file:fee193b50fa8dbda3e9dbec639709a18c062adef5add2fda1c8aa29e5a288d28 in / 
# Fri, 21 Feb 2020 22:30:18 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:30:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:30:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:30:36 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:07:12 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Sat, 22 Feb 2020 00:07:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:07:40 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Sat, 22 Feb 2020 00:08:42 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1203517876025e70b1c66491094cc6ea22704fd56a11f74043611ae5757a5180';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f216652dcc50778d13913dda73ea4b0f423fc0c6c45766fabac2e6f8b51d4b06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a44cddca5e072f3009e852344ce7e01755b87b60ae5cbb03232472db7c27536f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='654052eb2b2e8d95cceb443ac9863b5a038ebd29899b2b6e17825e9d0625b863';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='42345ba0e03b475e2e96336e5479ff94aed4a438002b193f3d3c4dff756c6b2c';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Sat, 22 Feb 2020 00:08:48 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:cfb81e1a655db6311df167d6e7259257ac1bec8fd6fa9eaef39c0661b1488490`  
		Last Modified: Fri, 21 Feb 2020 22:33:18 GMT  
		Size: 30.4 MB (30401091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a815faea808b955284818fc847eb2d542dc550d92f5974023b34000a33302aed`  
		Last Modified: Fri, 21 Feb 2020 22:33:12 GMT  
		Size: 35.2 KB (35207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e009f42ff24bbe56824bac50e1ba861b157cbf45a60e8e09ff1f4eee816a21a1`  
		Last Modified: Fri, 21 Feb 2020 22:33:11 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9164e4ca1b0934007f85d8baa8c3041d64dcde54ccfa21f38a106d1b876a1c21`  
		Last Modified: Fri, 21 Feb 2020 22:33:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ed5f62ef19e83fce216082c58e34647c04835dc77ff8bc04cabf8bc7eae7a`  
		Last Modified: Sat, 22 Feb 2020 00:11:32 GMT  
		Size: 3.1 MB (3093403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ad5fe977600e79c4e31fb3e778ef7e2612bb13024d5b93242d44f4a527c4cf`  
		Last Modified: Sat, 22 Feb 2020 00:11:50 GMT  
		Size: 143.3 MB (143305686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:latest` - linux; s390x

```console
$ docker pull ibmjava@sha256:7c3380ba3143f624dc7d912bb6c142a829d3c4d402c4423b051fb4c5d0f6f3a5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.6 MB (155630549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c3079d744cd9b63082cd800addd51241d6bcef9d19bac8d35d306f0fb3b49f5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:57:46 GMT
ADD file:7925c9b35ffa1870e7d336ddcdd6c3434715178c7d08ff2ce9796b651302c347 in / 
# Fri, 21 Feb 2020 21:57:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:57:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:57:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:57:53 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:31:02 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 22:31:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:31:16 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 22:32:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='1203517876025e70b1c66491094cc6ea22704fd56a11f74043611ae5757a5180';          YML_FILE='jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='f216652dcc50778d13913dda73ea4b0f423fc0c6c45766fabac2e6f8b51d4b06';          YML_FILE='jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='a44cddca5e072f3009e852344ce7e01755b87b60ae5cbb03232472db7c27536f';          YML_FILE='jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='654052eb2b2e8d95cceb443ac9863b5a038ebd29899b2b6e17825e9d0625b863';          YML_FILE='jre/linux/s390/index.yml';          ;;        s390x)          ESUM='42345ba0e03b475e2e96336e5479ff94aed4a438002b193f3d3c4dff756c6b2c';          YML_FILE='jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 22:32:20 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:b84fcb37dc33cf7416e0f1cf1219e16a15ab0d1c3aa4638d362f19c2679451de`  
		Last Modified: Fri, 21 Feb 2020 21:59:09 GMT  
		Size: 25.4 MB (25365672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9594931f903b7b3c4f5cb63196d29d715c50b567c128a5572131c12a25f04139`  
		Last Modified: Fri, 21 Feb 2020 21:59:06 GMT  
		Size: 36.2 KB (36186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66af13675c2330803d61d2198bb4f69c36bb7eed2d2b2bc3660fed8e873dce59`  
		Last Modified: Fri, 21 Feb 2020 21:59:11 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0fb7b2ee5c5bc387374bdd08f53541bdfcf678d9b9f83489c3923af65fed0`  
		Last Modified: Fri, 21 Feb 2020 21:59:21 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9381eb8b0a499263e6b76868e9412c47073e4d805bb897325f5e2de25846c6e7`  
		Last Modified: Fri, 21 Feb 2020 22:34:51 GMT  
		Size: 2.7 MB (2678898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aed53e3f9a4fd2569e95addcf56d9a518e7f39e0c6bfb15338120a65579742c`  
		Last Modified: Fri, 21 Feb 2020 22:35:01 GMT  
		Size: 127.5 MB (127548758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:sdk`

```console
$ docker pull ibmjava@sha256:e0b58c30610556cb0908fcf1881aabdd67642a10c209286723ba5944e629faf0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:sdk` - linux; amd64

```console
$ docker pull ibmjava@sha256:f6d1d9274601046eaef66bd217ad2ffb963c5f203af2bd8effbf331e7f3f5a59
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **197.2 MB (197164339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4083a7df6c6e099c1f3d01cf3ba89066c914712845cc94cbaa58405752cee5ad`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:17:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 23:18:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:18:02 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 23:20:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='a640a2fbdb3cef7faa68f9349060ca5f7ce403ca351c599f6bdd28ba0b9cfd8b';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='198a58f224d5d186c18f892e2372a8224fd20de876bf407a33b14e1992d6e1ff';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='16a0104383e0c3a1bcef066b15518ea1fdc91d630113297617b7c1a5a786f08b';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='deb2a801e04199711d66c2407c81c39b706afebe4eb6b5db864e8228c9f887c4';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='f70cb53a51e32fcbc6ccf367fbb7d23330fbf19d3c49e079efceb10403c7b470';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 23:20:32 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260c1687832ae34d925389a567f4eba8837fc1aa6be3f5f417b7342811950856`  
		Last Modified: Fri, 21 Feb 2020 23:20:53 GMT  
		Size: 3.0 MB (2965731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60a73079cba01de6bce06aaa395d4f2de238d0241f3bb5e5d51bb23b0f4ae5a`  
		Last Modified: Fri, 21 Feb 2020 23:21:35 GMT  
		Size: 167.5 MB (167470132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sdk` - linux; 386

```console
$ docker pull ibmjava@sha256:b70afef2aaeba2c1234e49be4e6461fdf47e27839e95c85dde035dc120d525fc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.0 MB (185957610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a52513788feb213292ade8b467e187d22646e43a8ce230be0581cd7081b3d84d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:39:03 GMT
ADD file:df203cc2574204629c69613fcea4942faa0f9224ff0c8bacb908b85d73604628 in / 
# Fri, 21 Feb 2020 21:39:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:39:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:39:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:39:06 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 21:55:45 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 21:55:54 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:54 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 21:58:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='a640a2fbdb3cef7faa68f9349060ca5f7ce403ca351c599f6bdd28ba0b9cfd8b';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='198a58f224d5d186c18f892e2372a8224fd20de876bf407a33b14e1992d6e1ff';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='16a0104383e0c3a1bcef066b15518ea1fdc91d630113297617b7c1a5a786f08b';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='deb2a801e04199711d66c2407c81c39b706afebe4eb6b5db864e8228c9f887c4';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='f70cb53a51e32fcbc6ccf367fbb7d23330fbf19d3c49e079efceb10403c7b470';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 21:58:17 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:ddc482e6a4fa5e364980052ab9f5d236f29ae9b217ed672b3dba44669f4041de`  
		Last Modified: Fri, 21 Feb 2020 21:39:58 GMT  
		Size: 27.1 MB (27123823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d2b8bf2fa50513ca7c508e44ac1a15c7ec42b1a3369a91380663868309ab46`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 34.6 KB (34625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84c193628e4067b419327ffa1bfef4b73161d9b1e3ce1e4ee83e714fd1d14e8`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271c42d486e4bb18cadbdf885d057c29384a032113047030f7c4bd6253bbf10`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d6ec2d33bfaf511d9237ee4ecaaf9d1f6b9aea99231bf1bdeb23a03997d84e`  
		Last Modified: Fri, 21 Feb 2020 21:58:25 GMT  
		Size: 3.0 MB (2992872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e13f152e74d140854578805c947c6351b0025a2cfd89c5f3be22b584b4e545`  
		Last Modified: Fri, 21 Feb 2020 21:59:10 GMT  
		Size: 155.8 MB (155805284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sdk` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:aaa45d323bb6551c7758ce7bd3049a60998851c57cf7ff5dede134001f64e627
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.1 MB (214118404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76aea1f3d48c97cbc3e845a9125b3d35a73c90df8f1d68cc272e97aa30f97ff3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:30:07 GMT
ADD file:fee193b50fa8dbda3e9dbec639709a18c062adef5add2fda1c8aa29e5a288d28 in / 
# Fri, 21 Feb 2020 22:30:18 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:30:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:30:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:30:36 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:07:12 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Sat, 22 Feb 2020 00:07:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:07:40 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Sat, 22 Feb 2020 00:11:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='a640a2fbdb3cef7faa68f9349060ca5f7ce403ca351c599f6bdd28ba0b9cfd8b';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='198a58f224d5d186c18f892e2372a8224fd20de876bf407a33b14e1992d6e1ff';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='16a0104383e0c3a1bcef066b15518ea1fdc91d630113297617b7c1a5a786f08b';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='deb2a801e04199711d66c2407c81c39b706afebe4eb6b5db864e8228c9f887c4';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='f70cb53a51e32fcbc6ccf367fbb7d23330fbf19d3c49e079efceb10403c7b470';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Sat, 22 Feb 2020 00:11:13 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:cfb81e1a655db6311df167d6e7259257ac1bec8fd6fa9eaef39c0661b1488490`  
		Last Modified: Fri, 21 Feb 2020 22:33:18 GMT  
		Size: 30.4 MB (30401091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a815faea808b955284818fc847eb2d542dc550d92f5974023b34000a33302aed`  
		Last Modified: Fri, 21 Feb 2020 22:33:12 GMT  
		Size: 35.2 KB (35207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e009f42ff24bbe56824bac50e1ba861b157cbf45a60e8e09ff1f4eee816a21a1`  
		Last Modified: Fri, 21 Feb 2020 22:33:11 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9164e4ca1b0934007f85d8baa8c3041d64dcde54ccfa21f38a106d1b876a1c21`  
		Last Modified: Fri, 21 Feb 2020 22:33:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ed5f62ef19e83fce216082c58e34647c04835dc77ff8bc04cabf8bc7eae7a`  
		Last Modified: Sat, 22 Feb 2020 00:11:32 GMT  
		Size: 3.1 MB (3093403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843d7c458af99a59c62f2e575db2982d334ad826bab5831bd1f814c942c71036`  
		Last Modified: Sat, 22 Feb 2020 00:12:47 GMT  
		Size: 180.6 MB (180587664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sdk` - linux; s390x

```console
$ docker pull ibmjava@sha256:0c5253c25629a7a767f58924384bff8548ed6cd909a087478633cf22d46f6b54
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **185.9 MB (185874896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adecfc855c63d3fd990bd40016886d53f102a0ebce14d4a1fd102de84b06f9af`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:57:46 GMT
ADD file:7925c9b35ffa1870e7d336ddcdd6c3434715178c7d08ff2ce9796b651302c347 in / 
# Fri, 21 Feb 2020 21:57:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:57:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:57:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:57:53 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:31:02 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 22:31:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:31:16 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 22:34:28 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='a640a2fbdb3cef7faa68f9349060ca5f7ce403ca351c599f6bdd28ba0b9cfd8b';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='198a58f224d5d186c18f892e2372a8224fd20de876bf407a33b14e1992d6e1ff';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='16a0104383e0c3a1bcef066b15518ea1fdc91d630113297617b7c1a5a786f08b';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='deb2a801e04199711d66c2407c81c39b706afebe4eb6b5db864e8228c9f887c4';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='f70cb53a51e32fcbc6ccf367fbb7d23330fbf19d3c49e079efceb10403c7b470';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 22:34:38 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:b84fcb37dc33cf7416e0f1cf1219e16a15ab0d1c3aa4638d362f19c2679451de`  
		Last Modified: Fri, 21 Feb 2020 21:59:09 GMT  
		Size: 25.4 MB (25365672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9594931f903b7b3c4f5cb63196d29d715c50b567c128a5572131c12a25f04139`  
		Last Modified: Fri, 21 Feb 2020 21:59:06 GMT  
		Size: 36.2 KB (36186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66af13675c2330803d61d2198bb4f69c36bb7eed2d2b2bc3660fed8e873dce59`  
		Last Modified: Fri, 21 Feb 2020 21:59:11 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0fb7b2ee5c5bc387374bdd08f53541bdfcf678d9b9f83489c3923af65fed0`  
		Last Modified: Fri, 21 Feb 2020 21:59:21 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9381eb8b0a499263e6b76868e9412c47073e4d805bb897325f5e2de25846c6e7`  
		Last Modified: Fri, 21 Feb 2020 22:34:51 GMT  
		Size: 2.7 MB (2678898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:188efe0c77413e1999ba1841b1b05ad7b5d34078c243847f9f2b1fe96f2cf66b`  
		Last Modified: Fri, 21 Feb 2020 22:35:34 GMT  
		Size: 157.8 MB (157793105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:sdk-alpine`

```console
$ docker pull ibmjava@sha256:f0cb037c1f3f2558743a8bcc96dcc995ed6c0f11532ef6265bbe7541a18b79f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `ibmjava:sdk-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:fc0783d65ae3c76f70acbc452036ecc12d44fd4efbba5bb4c55a1b7d294471b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.8 MB (175794023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:985a0bb7027890015088cfa7019fc3294f2f92ce21bdf5cbdb0bd8d2301da1f3`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 18:58:11 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 23 Jan 2020 18:58:11 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Thu, 23 Jan 2020 18:58:26 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Wed, 05 Feb 2020 02:15:32 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Wed, 05 Feb 2020 02:19:59 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='a640a2fbdb3cef7faa68f9349060ca5f7ce403ca351c599f6bdd28ba0b9cfd8b';          YML_FILE='sdk/linux/x86_64/index.yml';          ;;        i386)          ESUM='198a58f224d5d186c18f892e2372a8224fd20de876bf407a33b14e1992d6e1ff';          YML_FILE='sdk/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='16a0104383e0c3a1bcef066b15518ea1fdc91d630113297617b7c1a5a786f08b';          YML_FILE='sdk/linux/ppc64le/index.yml';          ;;        s390)          ESUM='deb2a801e04199711d66c2407c81c39b706afebe4eb6b5db864e8228c9f887c4';          YML_FILE='sdk/linux/s390/index.yml';          ;;        s390x)          ESUM='f70cb53a51e32fcbc6ccf367fbb7d23330fbf19d3c49e079efceb10403c7b470';          YML_FILE='sdk/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Wed, 05 Feb 2020 02:19:59 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56dae0f47127209aea70646977ebe366124ed65f82542cf651f109356bff110b`  
		Last Modified: Thu, 23 Jan 2020 19:01:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fad1ca64c34cb5644888bf2c8ae8fee9a4b1c9437b10bf8c0242dc13ce232a`  
		Last Modified: Thu, 23 Jan 2020 19:01:33 GMT  
		Size: 5.6 MB (5565608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4caa3d42c822b52e4a611f05d8ab9025fc59ce84b59e8d348f9e5071ea1d8d84`  
		Last Modified: Wed, 05 Feb 2020 02:25:32 GMT  
		Size: 167.4 MB (167440908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:sfj`

```console
$ docker pull ibmjava@sha256:2245db2f61875d55c4bf80e4d67651d0ee2e50cca9e67521475b48a4dbf93eb6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:sfj` - linux; amd64

```console
$ docker pull ibmjava@sha256:ca22e7111199088e1a47bbba293a778d6ef2be8d2cfb2b38dc58908b409a762c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.2 MB (93244430 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01e2f4d1bc75ac6e4da33b1a1fb5b51d9b69232c3d8b2bdf6c08d3247f7effaa`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:20:39 GMT
ADD file:91a750fb184711fde03c9172f41e8a907ccbb1bfb904c2c3f4ef595fcddbc3a9 in / 
# Fri, 21 Feb 2020 22:20:41 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:20:42 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:20:44 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:20:44 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 23:17:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 23:18:01 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 23:18:02 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 23:19:32 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bf7a6a9901ffab156683981546e75574f987973e03e839bb7249b918e314c4d8';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='d5982516f4e06468956ab89e084843c01ef08c3ed8e40378d33ebb586c92e9ce';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='c7d5cd7aa38879f88eda3e15ab6c1e76a5523522952b143cc2e9d971ef7876ed';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='a1ada0e17749fc87e187654e4b5a985c804397c00e4c3754494ec558d34ff738';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='429b0046251ca3c8ea663ee7fca4e07e35cbefb681977471e4bf5082590be160';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 23:19:32 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:423ae2b273f4c17ceee9e8482fa8d071d90c7d052ae208e1fe4963fceb3d6954`  
		Last Modified: Wed, 19 Feb 2020 13:21:21 GMT  
		Size: 26.7 MB (26692096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de83a2304fa1f7c4a13708a0d15b9704f5945c2be5cbb2b3ed9b2ccb718d0b3d`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 35.4 KB (35365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a83bce3af0648efaa60b9bb28225b09136d2d35d0bed25ac764297076dec1b`  
		Last Modified: Fri, 21 Feb 2020 22:22:49 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6b53be908de2c0c78070fff0a9f04835211b3156c4e73785747af365e71a0d7`  
		Last Modified: Fri, 21 Feb 2020 22:22:50 GMT  
		Size: 163.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260c1687832ae34d925389a567f4eba8837fc1aa6be3f5f417b7342811950856`  
		Last Modified: Fri, 21 Feb 2020 23:20:53 GMT  
		Size: 3.0 MB (2965731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a126cb7083d1eb53cc33b598084bdd4fec0c70d02553f6b33b97cf5399a3d996`  
		Last Modified: Fri, 21 Feb 2020 23:21:17 GMT  
		Size: 63.6 MB (63550223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; 386

```console
$ docker pull ibmjava@sha256:55279810cd6b7d49e3f831d6fb8dafeefec19d47861bc549eaf1892823c87fea
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.1 MB (93126563 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ac2f0b5e68ec69f1cc6e16c936eadaa2d348810a7c000e8969824498e6a21ee`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:39:03 GMT
ADD file:df203cc2574204629c69613fcea4942faa0f9224ff0c8bacb908b85d73604628 in / 
# Fri, 21 Feb 2020 21:39:04 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:39:05 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:39:05 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:39:06 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 21:55:45 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 21:55:54 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 21:55:54 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 21:57:21 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bf7a6a9901ffab156683981546e75574f987973e03e839bb7249b918e314c4d8';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='d5982516f4e06468956ab89e084843c01ef08c3ed8e40378d33ebb586c92e9ce';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='c7d5cd7aa38879f88eda3e15ab6c1e76a5523522952b143cc2e9d971ef7876ed';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='a1ada0e17749fc87e187654e4b5a985c804397c00e4c3754494ec558d34ff738';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='429b0046251ca3c8ea663ee7fca4e07e35cbefb681977471e4bf5082590be160';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 21:57:21 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:ddc482e6a4fa5e364980052ab9f5d236f29ae9b217ed672b3dba44669f4041de`  
		Last Modified: Fri, 21 Feb 2020 21:39:58 GMT  
		Size: 27.1 MB (27123823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d2b8bf2fa50513ca7c508e44ac1a15c7ec42b1a3369a91380663868309ab46`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 34.6 KB (34625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84c193628e4067b419327ffa1bfef4b73161d9b1e3ce1e4ee83e714fd1d14e8`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 844.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5271c42d486e4bb18cadbdf885d057c29384a032113047030f7c4bd6253bbf10`  
		Last Modified: Fri, 21 Feb 2020 21:39:52 GMT  
		Size: 162.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d6ec2d33bfaf511d9237ee4ecaaf9d1f6b9aea99231bf1bdeb23a03997d84e`  
		Last Modified: Fri, 21 Feb 2020 21:58:25 GMT  
		Size: 3.0 MB (2992872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3dd9a327e0abdb50631718508cb757e3929071d01a5340b2dfffa112bfc12d`  
		Last Modified: Fri, 21 Feb 2020 21:58:50 GMT  
		Size: 63.0 MB (62974237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:a82328b940a81f4f66b2578fb289ddcab849b18db2d38dd331d7cb710c0c63d4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.7 MB (101696182 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8216295d9cb9a9f807e939f49b2c988458cf287d7bfca6fa5eaacad4f32f475`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 22:30:07 GMT
ADD file:fee193b50fa8dbda3e9dbec639709a18c062adef5add2fda1c8aa29e5a288d28 in / 
# Fri, 21 Feb 2020 22:30:18 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 22:30:27 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 22:30:33 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 22:30:36 GMT
CMD ["/bin/bash"]
# Sat, 22 Feb 2020 00:07:12 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Sat, 22 Feb 2020 00:07:36 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Sat, 22 Feb 2020 00:07:40 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Sat, 22 Feb 2020 00:09:38 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bf7a6a9901ffab156683981546e75574f987973e03e839bb7249b918e314c4d8';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='d5982516f4e06468956ab89e084843c01ef08c3ed8e40378d33ebb586c92e9ce';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='c7d5cd7aa38879f88eda3e15ab6c1e76a5523522952b143cc2e9d971ef7876ed';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='a1ada0e17749fc87e187654e4b5a985c804397c00e4c3754494ec558d34ff738';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='429b0046251ca3c8ea663ee7fca4e07e35cbefb681977471e4bf5082590be160';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Sat, 22 Feb 2020 00:09:45 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:cfb81e1a655db6311df167d6e7259257ac1bec8fd6fa9eaef39c0661b1488490`  
		Last Modified: Fri, 21 Feb 2020 22:33:18 GMT  
		Size: 30.4 MB (30401091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a815faea808b955284818fc847eb2d542dc550d92f5974023b34000a33302aed`  
		Last Modified: Fri, 21 Feb 2020 22:33:12 GMT  
		Size: 35.2 KB (35207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e009f42ff24bbe56824bac50e1ba861b157cbf45a60e8e09ff1f4eee816a21a1`  
		Last Modified: Fri, 21 Feb 2020 22:33:11 GMT  
		Size: 852.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9164e4ca1b0934007f85d8baa8c3041d64dcde54ccfa21f38a106d1b876a1c21`  
		Last Modified: Fri, 21 Feb 2020 22:33:13 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667ed5f62ef19e83fce216082c58e34647c04835dc77ff8bc04cabf8bc7eae7a`  
		Last Modified: Sat, 22 Feb 2020 00:11:32 GMT  
		Size: 3.1 MB (3093403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fe9d4dfbb66823b78577dbae336c3673f800ffd00cb33cb78590fdaa78d18ec`  
		Last Modified: Sat, 22 Feb 2020 00:12:15 GMT  
		Size: 68.2 MB (68165442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:sfj` - linux; s390x

```console
$ docker pull ibmjava@sha256:cdfb5b3803e8b2845f1dd1e0bb5a1d8e4861055514102945c332f1c014ca337e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.8 MB (92771969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5c2f9c953d8d00a6e47802d9196805c2f8036b55d231804df5250a201fd2ecc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 21 Feb 2020 21:57:46 GMT
ADD file:7925c9b35ffa1870e7d336ddcdd6c3434715178c7d08ff2ce9796b651302c347 in / 
# Fri, 21 Feb 2020 21:57:50 GMT
RUN [ -z "$(apt-get indextargets)" ]
# Fri, 21 Feb 2020 21:57:51 GMT
RUN set -xe 		&& echo '#!/bin/sh' > /usr/sbin/policy-rc.d 	&& echo 'exit 101' >> /usr/sbin/policy-rc.d 	&& chmod +x /usr/sbin/policy-rc.d 		&& dpkg-divert --local --rename --add /sbin/initctl 	&& cp -a /usr/sbin/policy-rc.d /sbin/initctl 	&& sed -i 's/^exit.*/exit 0/' /sbin/initctl 		&& echo 'force-unsafe-io' > /etc/dpkg/dpkg.cfg.d/docker-apt-speedup 		&& echo 'DPkg::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' > /etc/apt/apt.conf.d/docker-clean 	&& echo 'APT::Update::Post-Invoke { "rm -f /var/cache/apt/archives/*.deb /var/cache/apt/archives/partial/*.deb /var/cache/apt/*.bin || true"; };' >> /etc/apt/apt.conf.d/docker-clean 	&& echo 'Dir::Cache::pkgcache ""; Dir::Cache::srcpkgcache "";' >> /etc/apt/apt.conf.d/docker-clean 		&& echo 'Acquire::Languages "none";' > /etc/apt/apt.conf.d/docker-no-languages 		&& echo 'Acquire::GzipIndexes "true"; Acquire::CompressionTypes::Order:: "gz";' > /etc/apt/apt.conf.d/docker-gzip-indexes 		&& echo 'Apt::AutoRemove::SuggestsImportant "false";' > /etc/apt/apt.conf.d/docker-autoremove-suggests
# Fri, 21 Feb 2020 21:57:53 GMT
RUN mkdir -p /run/systemd && echo 'docker' > /run/systemd/container
# Fri, 21 Feb 2020 21:57:53 GMT
CMD ["/bin/bash"]
# Fri, 21 Feb 2020 22:31:02 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 21 Feb 2020 22:31:15 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 21 Feb 2020 22:31:16 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Fri, 21 Feb 2020 22:33:10 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bf7a6a9901ffab156683981546e75574f987973e03e839bb7249b918e314c4d8';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='d5982516f4e06468956ab89e084843c01ef08c3ed8e40378d33ebb586c92e9ce';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='c7d5cd7aa38879f88eda3e15ab6c1e76a5523522952b143cc2e9d971ef7876ed';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='a1ada0e17749fc87e187654e4b5a985c804397c00e4c3754494ec558d34ff738';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='429b0046251ca3c8ea663ee7fca4e07e35cbefb681977471e4bf5082590be160';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 21 Feb 2020 22:33:15 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:b84fcb37dc33cf7416e0f1cf1219e16a15ab0d1c3aa4638d362f19c2679451de`  
		Last Modified: Fri, 21 Feb 2020 21:59:09 GMT  
		Size: 25.4 MB (25365672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9594931f903b7b3c4f5cb63196d29d715c50b567c128a5572131c12a25f04139`  
		Last Modified: Fri, 21 Feb 2020 21:59:06 GMT  
		Size: 36.2 KB (36186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66af13675c2330803d61d2198bb4f69c36bb7eed2d2b2bc3660fed8e873dce59`  
		Last Modified: Fri, 21 Feb 2020 21:59:11 GMT  
		Size: 847.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae0fb7b2ee5c5bc387374bdd08f53541bdfcf678d9b9f83489c3923af65fed0`  
		Last Modified: Fri, 21 Feb 2020 21:59:21 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9381eb8b0a499263e6b76868e9412c47073e4d805bb897325f5e2de25846c6e7`  
		Last Modified: Fri, 21 Feb 2020 22:34:51 GMT  
		Size: 2.7 MB (2678898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b471e3d97141df2f163d47de2e6222ce235a9476a72075db044277ae28c96f`  
		Last Modified: Fri, 21 Feb 2020 22:35:16 GMT  
		Size: 64.7 MB (64690178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `ibmjava:sfj-alpine`

```console
$ docker pull ibmjava@sha256:b00fffba2515014190e8ebb35535d2a19aecb531f53cb1235cf7b46543255a3f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `ibmjava:sfj-alpine` - linux; amd64

```console
$ docker pull ibmjava@sha256:21b66e7c20f804fc75e02c0b6d36f8ca3a89a9c30d5ea6ddf527c631d2a739cb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **71.9 MB (71917320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b289517bb3624bc26e9bcf388d2aa366c351bdc2600ed8b739944e5fbe55cc66`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 18:58:11 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Thu, 23 Jan 2020 18:58:11 GMT
COPY file:3ca1cc706ceed4c671485bfc9a5f46a78571aaf829b0ab9fbb88c9d48e27ccd3 in /etc/apk/keys 
# Thu, 23 Jan 2020 18:58:26 GMT
RUN apk add --no-cache --virtual .build-deps curl binutils     && GLIBC_VER="2.30-r0"     && ALPINE_GLIBC_REPO="https://github.com/sgerrand/alpine-pkg-glibc/releases/download"     && GCC_LIBS_URL="https://archive.archlinux.org/packages/g/gcc-libs/gcc-libs-8.2.1%2B20180831-1-x86_64.pkg.tar.xz"     && GCC_LIBS_SHA256=e4b39fb1f5957c5aab5c2ce0c46e03d30426f3b94b9992b009d417ff2d56af4d     && curl -fLs https://alpine-pkgs.sgerrand.com/sgerrand.rsa.pub -o /tmp/sgerrand.rsa.pub     && cmp -s /etc/apk/keys/sgerrand.rsa.pub /tmp/sgerrand.rsa.pub     && curl -fLs ${ALPINE_GLIBC_REPO}/${GLIBC_VER}/glibc-${GLIBC_VER}.apk > /tmp/${GLIBC_VER}.apk     && apk add /tmp/${GLIBC_VER}.apk     && curl -fLs ${GCC_LIBS_URL} -o /tmp/gcc-libs.tar.xz     && echo "${GCC_LIBS_SHA256}  /tmp/gcc-libs.tar.xz" | sha256sum -c -     && mkdir /tmp/gcc     && tar -xf /tmp/gcc-libs.tar.xz -C /tmp/gcc     && mv /tmp/gcc/usr/lib/libgcc* /tmp/gcc/usr/lib/libstdc++* /usr/glibc-compat/lib     && strip /usr/glibc-compat/lib/libgcc_s.so.* /usr/glibc-compat/lib/libstdc++.so*     && apk del --purge .build-deps     && apk add --no-cache ca-certificates openssl     && rm -rf /tmp/${GLIBC_VER}.apk /tmp/gcc /tmp/gcc-libs.tar.xz /var/cache/apk/* /tmp/*.pub
# Wed, 05 Feb 2020 02:15:32 GMT
ENV JAVA_VERSION=1.8.0_sr6fp5
# Wed, 05 Feb 2020 02:17:44 GMT
RUN set -eux;     apk --no-cache add --virtual .build-deps wget;     ARCH="$(apk --print-arch)";     case "${ARCH}" in        amd64|x86_64)          ESUM='bf7a6a9901ffab156683981546e75574f987973e03e839bb7249b918e314c4d8';          YML_FILE='sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='d5982516f4e06468956ab89e084843c01ef08c3ed8e40378d33ebb586c92e9ce';          YML_FILE='sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='c7d5cd7aa38879f88eda3e15ab6c1e76a5523522952b143cc2e9d971ef7876ed';          YML_FILE='sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='a1ada0e17749fc87e187654e4b5a985c804397c00e4c3754494ec558d34ff738';          YML_FILE='sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='429b0046251ca3c8ea663ee7fca4e07e35cbefb681977471e4bf5082590be160';          YML_FILE='sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;     apk del .build-deps;
# Wed, 05 Feb 2020 02:17:44 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56dae0f47127209aea70646977ebe366124ed65f82542cf651f109356bff110b`  
		Last Modified: Thu, 23 Jan 2020 19:01:31 GMT  
		Size: 545.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fad1ca64c34cb5644888bf2c8ae8fee9a4b1c9437b10bf8c0242dc13ce232a`  
		Last Modified: Thu, 23 Jan 2020 19:01:33 GMT  
		Size: 5.6 MB (5565608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2e2c0a8d924df9316c50e4bc8eab430b8c2c6057ac72d2ca006ca712403d3f`  
		Last Modified: Wed, 05 Feb 2020 02:22:28 GMT  
		Size: 63.6 MB (63564205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
