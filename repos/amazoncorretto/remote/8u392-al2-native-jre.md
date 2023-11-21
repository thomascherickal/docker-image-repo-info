## `amazoncorretto:8u392-al2-native-jre`

```console
$ docker pull amazoncorretto@sha256:b91876e04673a1f3f23d29f93e3323e1b83720e999de66bd80e648346a106871
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u392-al2-native-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:737e4a6d3893f6d0e1ca227dd2bd61822d84ba2c2749c875027eb99a71120b33
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.8 MB (171786060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4bb152601c4a6594a938f624f0388749d7c3a276bf5290ae8c354924dfc1850`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:21:54 GMT
COPY dir:ddf8ce4c235ebf92718d40c0041035b283a61cbd94b49610e57999ebc78d3ec6 in / 
# Tue, 21 Nov 2023 03:21:55 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 04:13:06 GMT
ARG version=1.8.0_392.b08-1
# Tue, 21 Nov 2023 04:14:43 GMT
# ARGS: version=1.8.0_392.b08-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.' | tr '_' '.'| tr -d "b" | awk -F. '{print $2"."$4"."$5"."$6}')     && rpm --import /etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2     && echo "localpkg_gpgcheck=1" >> /etc/yum.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-1.8.0-amazon-corretto-$version.amzn2.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && echo $(rpm -K "${CORRETO_TEMP}/${rpm}")     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: rsa sha1 (md5) pgp md5 OK" || exit 1;     done     && yum install -y $(yum deplist ${CORRETO_TEMP}/*.rpm |grep provider | grep -v log4j-cve | tr -s ' ' |cut -d ' ' -f 3 )     && rpm -i --nodeps ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-1.8.0-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && yum clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/yum.conf
# Tue, 21 Nov 2023 04:14:44 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 04:14:44 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto/jre
```

-	Layers:
	-	`sha256:0b4a6f011995244a95bff79a1298e83d230bc0aa22871a9c510745cafebec227`  
		Last Modified: Sun, 19 Nov 2023 03:18:53 GMT  
		Size: 62.6 MB (62641917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e28f0306b40def70c987ebbfe1b6e8915d00e905a2817d6bd1d9700e0675ce`  
		Last Modified: Tue, 21 Nov 2023 04:27:02 GMT  
		Size: 109.1 MB (109144143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u392-al2-native-jre` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:3c6322801fe0982aef17cc9ee68879bba22384b2badb7b496af82657ee13bfc3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.2 MB (117215910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3f57794ef93526b1662ca97f42456608121d7c2e5303e036f634b726bd2e2a6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:39:49 GMT
COPY dir:21fc61c0ea1d6a14f556bdbd5029389644807e82a8de54f60438fc773e3e2465 in / 
# Tue, 21 Nov 2023 03:39:51 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 05:07:17 GMT
ARG version=1.8.0_392.b08-1
# Tue, 21 Nov 2023 05:08:12 GMT
# ARGS: version=1.8.0_392.b08-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.' | tr '_' '.'| tr -d "b" | awk -F. '{print $2"."$4"."$5"."$6}')     && rpm --import /etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2     && echo "localpkg_gpgcheck=1" >> /etc/yum.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-1.8.0-amazon-corretto-$version.amzn2.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && echo $(rpm -K "${CORRETO_TEMP}/${rpm}")     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: rsa sha1 (md5) pgp md5 OK" || exit 1;     done     && yum install -y $(yum deplist ${CORRETO_TEMP}/*.rpm |grep provider | grep -v log4j-cve | tr -s ' ' |cut -d ' ' -f 3 )     && rpm -i --nodeps ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-1.8.0-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && yum clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/yum.conf
# Tue, 21 Nov 2023 05:08:12 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 05:08:12 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto/jre
```

-	Layers:
	-	`sha256:ae50e077554aa1fe734206cc35e32dc0b0389a0ff7aa8d08626157b225100b42`  
		Last Modified: Mon, 20 Nov 2023 21:52:59 GMT  
		Size: 64.4 MB (64424056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db1289817c9a6ca232305bea483ebe9c631abe5886749b6917d6f3ba4e0a60d`  
		Last Modified: Tue, 21 Nov 2023 05:17:41 GMT  
		Size: 52.8 MB (52791854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
