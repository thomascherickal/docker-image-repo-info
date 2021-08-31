## `ibmjava:8-sfj`

```console
$ docker pull ibmjava@sha256:1426b37092f46c54e20d0da0bd6442093d5bc2d844e98725ba945f9ed03c4a60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `ibmjava:8-sfj` - linux; amd64

```console
$ docker pull ibmjava@sha256:29adf4205e8d886c6b9a6115198214a3ea2b89997b800c4afb40b30ebc97f14a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.0 MB (94011255 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37410eb8b00b522cd8b08d1ac01a1924e70a359fc7a752476e03571d33543cbc`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:30 GMT
ADD file:e729fb032bd2f7cde20fb343da0cd358447e8b23028422c123944e8d0be660fa in / 
# Mon, 26 Jul 2021 21:21:31 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 23:22:54 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Mon, 26 Jul 2021 23:23:02 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Aug 2021 17:20:00 GMT
ENV JAVA_VERSION=8.0.6.35
# Fri, 13 Aug 2021 17:21:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d9ad4dd78cde42b44a0e9ba91d6b85fb134b56fb30ef0009153cfba54778978e';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='59ada28d2bd89365f0eaf259cf587b9e9605c8407394e2945f84e574b94e0134';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='5e8adf7a5064549f06eb864dfea1d94a1e7fd96f1a971b8575b02593a15cb0c4';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='98f091cf8228282f0b116ea8958129290f659ac360cf05f606ac3dfef3548a85';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='201faefc1f6b47d045889ff1610f70d09fdb07d1d4aa062cba8b32d41cd233b4';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 13 Aug 2021 17:21:45 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:feac5306138255e28a9862d3f3d29025d0a4d0648855afe1acd6131af07138ac`  
		Last Modified: Mon, 26 Jul 2021 21:22:52 GMT  
		Size: 26.7 MB (26709039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcc8b59a59a15868e1ba8f0176e149949b7fa1f2c69f90ad72eb7270fdc65f7`  
		Last Modified: Mon, 26 Jul 2021 23:26:50 GMT  
		Size: 3.0 MB (2958819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68f5756b26d7dfa1cb2ff781f8c57f529a1ffb5b06ae9a68ef73edd6c06db78`  
		Last Modified: Fri, 13 Aug 2021 17:25:04 GMT  
		Size: 64.3 MB (64343397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; 386

```console
$ docker pull ibmjava@sha256:887c9f2ce25e600a5bf4be416955305e4b861c43dc3d3825e0af284c60f6f4bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.9 MB (93877342 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:decfb9ce4e6e2e91f7d3f01135f7b771a0d081dc5e4c54e2b8f376c4d3745737`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:39:08 GMT
ADD file:615269b4e3662feffa9257a896456387554777532f070eae2226fa704e50150e in / 
# Tue, 31 Aug 2021 01:39:08 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:12:23 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 02:12:31 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:12:31 GMT
ENV JAVA_VERSION=8.0.6.35
# Tue, 31 Aug 2021 02:13:45 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d9ad4dd78cde42b44a0e9ba91d6b85fb134b56fb30ef0009153cfba54778978e';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='59ada28d2bd89365f0eaf259cf587b9e9605c8407394e2945f84e574b94e0134';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='5e8adf7a5064549f06eb864dfea1d94a1e7fd96f1a971b8575b02593a15cb0c4';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='98f091cf8228282f0b116ea8958129290f659ac360cf05f606ac3dfef3548a85';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='201faefc1f6b47d045889ff1610f70d09fdb07d1d4aa062cba8b32d41cd233b4';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Aug 2021 02:13:45 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:01a6f9651a524383d1aac8b05ceaf7a079d305146c6bf120b7ffb27247b18230`  
		Last Modified: Tue, 31 Aug 2021 01:40:06 GMT  
		Size: 27.2 MB (27162437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2dc5982ecfcf15c732820dee42795101949b64c04ef86dc8296f7b9a16509d4`  
		Last Modified: Tue, 31 Aug 2021 02:15:07 GMT  
		Size: 3.0 MB (2989388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd587741057be9756d70f8ab18d1125a760b56daa6b8a5cae94927e996a66d25`  
		Last Modified: Tue, 31 Aug 2021 02:15:44 GMT  
		Size: 63.7 MB (63725517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; ppc64le

```console
$ docker pull ibmjava@sha256:5a537246fff29822f19800ee865e6f334cfc4459f4ca023958a829991082e1b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (98047551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98c8d49302a905fa41939efa41d1b453a8be938fe9059abbf5ed60d6f0f9ec73`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:12:31 GMT
ADD file:2e6f05bbffb47b3ea8e5e4127452e80debc89fb9e22af2dc5c735ea579adad64 in / 
# Mon, 26 Jul 2021 23:12:34 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 01:55:55 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 27 Jul 2021 01:56:51 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Fri, 13 Aug 2021 17:16:48 GMT
ENV JAVA_VERSION=8.0.6.35
# Fri, 13 Aug 2021 17:19:03 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d9ad4dd78cde42b44a0e9ba91d6b85fb134b56fb30ef0009153cfba54778978e';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='59ada28d2bd89365f0eaf259cf587b9e9605c8407394e2945f84e574b94e0134';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='5e8adf7a5064549f06eb864dfea1d94a1e7fd96f1a971b8575b02593a15cb0c4';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='98f091cf8228282f0b116ea8958129290f659ac360cf05f606ac3dfef3548a85';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='201faefc1f6b47d045889ff1610f70d09fdb07d1d4aa062cba8b32d41cd233b4';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Fri, 13 Aug 2021 17:19:07 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:3c742a0b2a0025420dcf1bc91d81de2ffb292328fad483ce715521d725503b66`  
		Last Modified: Mon, 26 Jul 2021 23:15:30 GMT  
		Size: 30.4 MB (30437958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274a7ceecd631ec4df912a3b0382831ab0f4d2796b455732587f4678f12dc8d8`  
		Last Modified: Tue, 27 Jul 2021 02:03:19 GMT  
		Size: 3.1 MB (3083057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0134f6bf2485178363e983f5bf438d0cd4220d27e69ff6c443944c5162041f2b`  
		Last Modified: Fri, 13 Aug 2021 17:21:52 GMT  
		Size: 64.5 MB (64526536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `ibmjava:8-sfj` - linux; s390x

```console
$ docker pull ibmjava@sha256:81b010776718b38d7480d1921514b907df374deb08b6f9d8d4ee5d2829056489
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.4 MB (93411032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24d11a7b7b65fcd918375630840f85095ae607331d52e0e893f5428a9659453f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 31 Aug 2021 01:42:06 GMT
ADD file:587feabbf5ad530bb19e438490116110e0c3f5fd5c8b98bcce6767af928c66de in / 
# Tue, 31 Aug 2021 01:42:10 GMT
CMD ["bash"]
# Tue, 31 Aug 2021 02:00:34 GMT
MAINTAINER Jayashree Gopi <jayasg12@in.ibm.com> (@jayasg12)
# Tue, 31 Aug 2021 02:00:47 GMT
RUN apt-get update     && apt-get install -y --no-install-recommends wget ca-certificates     && rm -rf /var/lib/apt/lists/*
# Tue, 31 Aug 2021 02:00:48 GMT
ENV JAVA_VERSION=8.0.6.35
# Tue, 31 Aug 2021 02:02:30 GMT
RUN set -eux;     ARCH="$(dpkg --print-architecture)";     case "${ARCH}" in        amd64|x86_64)          ESUM='d9ad4dd78cde42b44a0e9ba91d6b85fb134b56fb30ef0009153cfba54778978e';          YML_FILE='8.0/sfj/linux/x86_64/index.yml';          ;;        i386)          ESUM='59ada28d2bd89365f0eaf259cf587b9e9605c8407394e2945f84e574b94e0134';          YML_FILE='8.0/sfj/linux/i386/index.yml';          ;;        ppc64el|ppc64le)          ESUM='5e8adf7a5064549f06eb864dfea1d94a1e7fd96f1a971b8575b02593a15cb0c4';          YML_FILE='8.0/sfj/linux/ppc64le/index.yml';          ;;        s390)          ESUM='98f091cf8228282f0b116ea8958129290f659ac360cf05f606ac3dfef3548a85';          YML_FILE='8.0/sfj/linux/s390/index.yml';          ;;        s390x)          ESUM='201faefc1f6b47d045889ff1610f70d09fdb07d1d4aa062cba8b32d41cd233b4';          YML_FILE='8.0/sfj/linux/s390x/index.yml';          ;;        *)          echo "Unsupported arch: ${ARCH}";          exit 1;          ;;     esac;     BASE_URL="https://public.dhe.ibm.com/ibmdl/export/pub/systems/cloud/runtimes/java/meta/";     wget -q -U UA_IBM_JAVA_Docker -O /tmp/index.yml ${BASE_URL}/${YML_FILE};     JAVA_URL=$(sed -n '/^'${JAVA_VERSION}:'/{n;s/\s*uri:\s//p}'< /tmp/index.yml);     wget -q -U UA_IBM_JAVA_Docker -O /tmp/ibm-java.bin ${JAVA_URL};     echo "${ESUM}  /tmp/ibm-java.bin" | sha256sum -c -;     echo "INSTALLER_UI=silent" > /tmp/response.properties;     echo "USER_INSTALL_DIR=/opt/ibm/java" >> /tmp/response.properties;     echo "LICENSE_ACCEPTED=TRUE" >> /tmp/response.properties;     mkdir -p /opt/ibm;     chmod +x /tmp/ibm-java.bin;     /tmp/ibm-java.bin -i silent -f /tmp/response.properties;     rm -f /tmp/response.properties;     rm -f /tmp/index.yml;     rm -f /tmp/ibm-java.bin;
# Tue, 31 Aug 2021 02:02:35 GMT
ENV JAVA_HOME=/opt/ibm/java/jre PATH=/opt/ibm/java/jre/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin IBM_JAVA_OPTIONS=-XX:+UseContainerSupport
```

-	Layers:
	-	`sha256:8a5845e3ee3e2d93d3bcf0f827afe41d646f59cdf52f107306c232b60ffeb3a4`  
		Last Modified: Tue, 31 Aug 2021 01:43:59 GMT  
		Size: 25.4 MB (25366401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3910b4a125e933281c490aa153e2a43cf8e21bbe2142e9491a5c3004481598c9`  
		Last Modified: Tue, 31 Aug 2021 02:06:15 GMT  
		Size: 2.7 MB (2677633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90483140c8323edda00aa1cb79960f1c07e4689eea1184fea844f457a64a536c`  
		Last Modified: Tue, 31 Aug 2021 02:06:41 GMT  
		Size: 65.4 MB (65366998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
