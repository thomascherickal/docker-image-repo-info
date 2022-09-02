## `ibmjava:8-sfj`

```console
$ docker pull ibmjava@sha256:95b600d7a783c3e50e237d047932aff382e8327f9bc99fb4fde52e5072106157
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-sfj` - linux; amd64

```console
$ docker pull ibmjava@sha256:41df0dd965c8a61c21a7bb2dae361d8a0b7fea88fa9db1f8406aec3bd2b019f3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.7 MB (94688195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9472ee3cbc38be63ac9f02c403ac9c2c95b0d59a2db85d6f593abf22677713f`
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
# Fri, 02 Sep 2022 03:34:54 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='3b3760f9f5ec720bcfee6e2a21cfe3e7d3539513ebd9e51e1a1b9998bb768c7a';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='c7e3ddae49d67eae37a70e48593214e8387aa07599479a22b2cfd1e3eb73aae0';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='820a906fbd7dd8b6d91ef8573376080e7596e9c70eb87d052b08a48bfa1eda79';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='052f7c06e16187b123b5e3007ed39c2b14176fcd7ae9b9da029469fe57da69d8';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='f9cb898fce2b3c2a384db5e998a73007265a5f45c11a0cee13e742fc84311c52';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 02 Sep 2022 03:34:54 GMT
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
	-	`sha256:86141b0359b392107dde7767d0ecf56e543f6aa88d5378fa4056c2f14f317570`  
		Last Modified: Fri, 02 Sep 2022 03:37:03 GMT  
		Size: 65.0 MB (65020267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; 386

```console
$ docker pull ibmjava@sha256:d1b4948e97b30bb8099e3a0b8dde7367351aee27951971b4ba601bf1732c1949
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94531815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51e8f779dd1f55f94f43e49df6ce170a043bef1b74c37b65fb7f381398480867`
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
# Fri, 02 Sep 2022 02:45:43 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='3b3760f9f5ec720bcfee6e2a21cfe3e7d3539513ebd9e51e1a1b9998bb768c7a';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='c7e3ddae49d67eae37a70e48593214e8387aa07599479a22b2cfd1e3eb73aae0';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='820a906fbd7dd8b6d91ef8573376080e7596e9c70eb87d052b08a48bfa1eda79';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='052f7c06e16187b123b5e3007ed39c2b14176fcd7ae9b9da029469fe57da69d8';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='f9cb898fce2b3c2a384db5e998a73007265a5f45c11a0cee13e742fc84311c52';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 02 Sep 2022 02:45:43 GMT
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
	-	`sha256:7b3cb403c14e6f6520d28fb4e4b550932b16ad0b497ea073468c2c780f0fa181`  
		Last Modified: Fri, 02 Sep 2022 02:47:56 GMT  
		Size: 64.4 MB (64384315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:dd72846d3c1d6ee68f3c2f1ae72be0af92ac90cf8507f1eed0543b5a93d908a4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.8 MB (98752540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8d6a38a82258e2c18e442f7c87e78f902faa01d07c4fdada5b6e3c3f5a75396`
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
# Fri, 26 Aug 2022 19:21:22 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='3b3760f9f5ec720bcfee6e2a21cfe3e7d3539513ebd9e51e1a1b9998bb768c7a';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='c7e3ddae49d67eae37a70e48593214e8387aa07599479a22b2cfd1e3eb73aae0';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='820a906fbd7dd8b6d91ef8573376080e7596e9c70eb87d052b08a48bfa1eda79';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='052f7c06e16187b123b5e3007ed39c2b14176fcd7ae9b9da029469fe57da69d8';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='f9cb898fce2b3c2a384db5e998a73007265a5f45c11a0cee13e742fc84311c52';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 26 Aug 2022 19:21:23 GMT
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
	-	`sha256:f12c134638b4339cc91ca3ed409c3a37e27a76d32874d1c4915870acc4925981`  
		Last Modified: Fri, 26 Aug 2022 19:25:55 GMT  
		Size: 65.2 MB (65235127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; s390x

```console
$ docker pull ibmjava@sha256:a8dfe96833d78da87aa64bfed89d9f5a5f46cda27e6df85f470848675faf3c82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94160727 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:447880bd833075364cd8d910f0ecd7fcbc26c7edbdc3779123720007e9d88453`
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
# Fri, 02 Sep 2022 01:34:05 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='3b3760f9f5ec720bcfee6e2a21cfe3e7d3539513ebd9e51e1a1b9998bb768c7a';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='c7e3ddae49d67eae37a70e48593214e8387aa07599479a22b2cfd1e3eb73aae0';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='820a906fbd7dd8b6d91ef8573376080e7596e9c70eb87d052b08a48bfa1eda79';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='052f7c06e16187b123b5e3007ed39c2b14176fcd7ae9b9da029469fe57da69d8';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='f9cb898fce2b3c2a384db5e998a73007265a5f45c11a0cee13e742fc84311c52';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 02 Sep 2022 01:34:07 GMT
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
	-	`sha256:2db07ed0f29817295dda0b595a12f89590e2360bc2806adb967d82da7b2dc757`  
		Last Modified: Fri, 02 Sep 2022 01:36:07 GMT  
		Size: 66.1 MB (66119510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
