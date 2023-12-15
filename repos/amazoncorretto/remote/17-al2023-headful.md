## `amazoncorretto:17-al2023-headful`

```console
$ docker pull amazoncorretto@sha256:8c4e2d4dcfb11623e4a8a740ad64465852ef047546440cc6de58155a5bde172e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-al2023-headful` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:ae84633b09ecc7c80f873ba744b2aa7498d6aabadc9ae494c1b846049e7a0690
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135229537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a551bb92f22c9c1558fcc2eaf9df9042156be4b66c3c7a52a67d21f06081cf12`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 15 Dec 2023 20:22:29 GMT
COPY dir:6a0327957e10cfc5aab398cafdbbdbefb52a510a0fb73d8bf1952a36ff5452a4 in / 
# Fri, 15 Dec 2023 20:22:30 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 20:46:21 GMT
ARG version=17.0.9.8-1
# Fri, 15 Dec 2023 20:46:21 GMT
ARG package_version=1
# Fri, 15 Dec 2023 20:47:26 GMT
# ARGS: package_version=1 version=17.0.9.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 15 Dec 2023 20:47:27 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 20:47:27 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:97668dd20d4358bee95dea91ba9ca63bae56f3a5759ca22763c5940071e14884`  
		Last Modified: Fri, 15 Dec 2023 01:53:15 GMT  
		Size: 52.2 MB (52221241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311db123cfc207be2bb8ef8398915b1336dc64ec74e379edaab0965dd55c29e6`  
		Last Modified: Fri, 15 Dec 2023 20:58:12 GMT  
		Size: 83.0 MB (83008296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-al2023-headful` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:b803e3ce3787505477d50fa36160140127df9e8aacf6d60239f42bb4884d9f67
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.7 MB (133652210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c5187cceb9c1b86acba122247db8cdebf43c685de03875ac10c0454d39bc6d1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 15 Dec 2023 20:44:19 GMT
COPY dir:02d504631605340a0b119cb2fbfb77790d9edc1c5c4eae4b1c4c4761f2d76905 in / 
# Fri, 15 Dec 2023 20:44:20 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 21:13:20 GMT
ARG version=17.0.9.8-1
# Fri, 15 Dec 2023 21:13:20 GMT
ARG package_version=1
# Fri, 15 Dec 2023 21:14:13 GMT
# ARGS: package_version=1 version=17.0.9.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 15 Dec 2023 21:14:14 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 21:14:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:ce0da89e7bfb7e6039e531a7f8bb3d39522916880c6425022b0ab8562dea66c3`  
		Last Modified: Fri, 15 Dec 2023 01:53:13 GMT  
		Size: 51.3 MB (51304607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883681af56f2db3d6f1369e9d2aa5e7817b476a7f1f6c014be207bda6572adc5`  
		Last Modified: Fri, 15 Dec 2023 21:22:55 GMT  
		Size: 82.3 MB (82347603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
