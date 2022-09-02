## `ibmjava:latest`

```console
$ docker pull ibmjava@sha256:90903173558ddf502a26dc5e46feb89a0ed4ae50c0e72305379329fdda3101a9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:latest` - linux; amd64

```console
$ docker pull ibmjava@sha256:feb1d7e0acbf1b7845dc432572e23064a74ca065119c58f1ba729a080c0c487e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.0 MB (159010074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fee2a2c8d157e6c3838f6090f24ea51974f8bf31753eae8d9b666f25394be77d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:46:18 GMT
ADD file:8b379a8fd96e76d10db6f9ae4e9675de33d227db0431ca2a7ca799119e905e8f in / 
# Thu, 01 Sep 2022 23:46:18 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 03:33:09 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 02 Sep 2022 03:33:18 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 03:33:18 GMT
ENV JAVA_VERSION=8.0.7.15
# Fri, 02 Sep 2022 03:34:09 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='b789e740367f1c01581135052b66f35dff8c2cc780cdaeaa5075b5578d3e8e42';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='96c3433896f36f7c3f088c42629350778e13b878162d498d2f8df4e5b806d2cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='379517c106ff3e93f09f8b05821c8f98ddd7446a29d28f35a447f51e7fc4ce47';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='09c7c778c8163085a027e37f0f73a7142e7da77b921bc662c06f7fce223fa989';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='658d719236698b775def5f3b6643641db333d59b1729af51aa5f35da7144868e';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 02 Sep 2022 03:34:10 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:dad0f37c70a668d101c86b5c769d452ff29c6d51f811891384cc7da00fce192f`  
		Last Modified: Wed, 31 Aug 2022 06:57:55 GMT  
		Size: 26.7 MB (26710085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:157830093eea5fa46b30d4135fd942c7664880357dd7417359d97eb1a68cf09a`  
		Last Modified: Fri, 02 Sep 2022 03:36:34 GMT  
		Size: 3.0 MB (2957843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e878949a754d958979ecdf2fa9b28074473049ad58d7bd32a63d0da4818362b9`  
		Last Modified: Fri, 02 Sep 2022 03:36:44 GMT  
		Size: 129.3 MB (129342146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:latest` - linux; 386

```console
$ docker pull ibmjava@sha256:45c437e035097dea9b0c00f6ea3dfe9689b01ea7af3df1f38d7f9c73d9f3f3ab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.6 MB (147610221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30113a2c5810104bc783824f3420b9ac7e559f70cd209d462f6ed78333255c58`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 01 Sep 2022 23:53:52 GMT
ADD file:93fdf10efcfc26ed4b10659ddc78284113a38c500811d27ffc41de25e2c9b4ab in / 
# Thu, 01 Sep 2022 23:53:53 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 02:43:53 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 02 Sep 2022 02:44:04 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 02:44:05 GMT
ENV JAVA_VERSION=8.0.7.15
# Fri, 02 Sep 2022 02:44:56 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='b789e740367f1c01581135052b66f35dff8c2cc780cdaeaa5075b5578d3e8e42';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='96c3433896f36f7c3f088c42629350778e13b878162d498d2f8df4e5b806d2cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='379517c106ff3e93f09f8b05821c8f98ddd7446a29d28f35a447f51e7fc4ce47';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='09c7c778c8163085a027e37f0f73a7142e7da77b921bc662c06f7fce223fa989';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='658d719236698b775def5f3b6643641db333d59b1729af51aa5f35da7144868e';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 02 Sep 2022 02:44:56 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:e09c10b62acdd55abc0548e8b24a3f314d657a49d5b9e4714ae753238c982a61`  
		Last Modified: Thu, 01 Sep 2022 23:54:38 GMT  
		Size: 27.2 MB (27164218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fe212f9b4880824cc2696387d260a467809dc297143da6c39649d2686eb090`  
		Last Modified: Fri, 02 Sep 2022 02:47:21 GMT  
		Size: 3.0 MB (2983282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9815912868b0d90329685901026b47700f9aae2655dcbe4775c9598aa528cfe7`  
		Last Modified: Fri, 02 Sep 2022 02:47:34 GMT  
		Size: 117.5 MB (117462721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:latest` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:5adc59a78a71a51002e2422e59defb3084a9339aa30fb54acf018a2318e26041
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **162.4 MB (162412482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c153f6fec2349df07565406ea5f5563a153be3673c7622b87f48b5eebfd648`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:30:50 GMT
ADD file:32fc7b9b5853c93c45b1a96054c30104fd200ac7d40d0388aff736c478f917cb in / 
# Tue, 02 Aug 2022 01:30:52 GMT
CMD ["bash"]
# Wed, 03 Aug 2022 03:44:16 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Wed, 03 Aug 2022 03:44:53 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 26 Aug 2022 19:16:47 GMT
ENV JAVA_VERSION=8.0.7.15
# Fri, 26 Aug 2022 19:19:16 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='b789e740367f1c01581135052b66f35dff8c2cc780cdaeaa5075b5578d3e8e42';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='96c3433896f36f7c3f088c42629350778e13b878162d498d2f8df4e5b806d2cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='379517c106ff3e93f09f8b05821c8f98ddd7446a29d28f35a447f51e7fc4ce47';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='09c7c778c8163085a027e37f0f73a7142e7da77b921bc662c06f7fce223fa989';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='658d719236698b775def5f3b6643641db333d59b1729af51aa5f35da7144868e';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Aug 2022 19:19:19 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:1a9ff13e38cae7994b55e6db5c3d190d2b7a03043ae238a6f71a285376de46bb`  
		Last Modified: Tue, 02 Aug 2022 01:33:07 GMT  
		Size: 30.4 MB (30441470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99970d1735353adabddaef52faa1237908c9cdf39198088cf543cb21ecb3fa69`  
		Last Modified: Wed, 03 Aug 2022 03:52:54 GMT  
		Size: 3.1 MB (3075943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9501b5b22fed4db7ff494e125e8d08db9f15c579219c407c9707f7051a82644`  
		Last Modified: Fri, 26 Aug 2022 19:25:25 GMT  
		Size: 128.9 MB (128895069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:latest` - linux; s390x

```console
$ docker pull ibmjava@sha256:c37de7230c1126e4b2168f67164f5c5b47f447980408f29f4abb2759d9505778
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154502102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04edf91ea55e7f7bd3c589de21feb53d708107423e6f83ea9e9562b6bdb7a3e3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 02 Sep 2022 01:03:02 GMT
ADD file:ee88f505cbf59825aed59486848971d1be33d8cc49f3a1df647a1486f310405f in / 
# Fri, 02 Sep 2022 01:03:04 GMT
CMD ["bash"]
# Fri, 02 Sep 2022 01:32:24 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Fri, 02 Sep 2022 01:32:34 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 02 Sep 2022 01:32:34 GMT
ENV JAVA_VERSION=8.0.7.15
# Fri, 02 Sep 2022 01:33:22 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='b789e740367f1c01581135052b66f35dff8c2cc780cdaeaa5075b5578d3e8e42';          YML_FILE='8.0/jre/linux/x86_64/index.yml';          ;;        i386)          ESUM='96c3433896f36f7c3f088c42629350778e13b878162d498d2f8df4e5b806d2cd';          YML_FILE='8.0/jre/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='379517c106ff3e93f09f8b05821c8f98ddd7446a29d28f35a447f51e7fc4ce47';          YML_FILE='8.0/jre/linux/ppc64le/index.yml';          ;;        s390)          ESUM='09c7c778c8163085a027e37f0f73a7142e7da77b921bc662c06f7fce223fa989';          YML_FILE='8.0/jre/linux/s390/index.yml';          ;;        s390x)          ESUM='658d719236698b775def5f3b6643641db333d59b1729af51aa5f35da7144868e';          YML_FILE='8.0/jre/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 02 Sep 2022 01:33:24 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:f98934bea0e17bc3e47aa5c2cb45f3bbcf512fd6211b763c88da22fffe217709`  
		Last Modified: Fri, 02 Sep 2022 01:04:37 GMT  
		Size: 25.4 MB (25369467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d507efb7c83fc179172edf420da4401fe01a9da3de58f6f26a15c75545dc9a`  
		Last Modified: Fri, 02 Sep 2022 01:35:42 GMT  
		Size: 2.7 MB (2671750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aca6f543b381e1e251440926a1b6aa538293e755dba9a0a3f14944fabe90451`  
		Last Modified: Fri, 02 Sep 2022 01:35:51 GMT  
		Size: 126.5 MB (126460885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
