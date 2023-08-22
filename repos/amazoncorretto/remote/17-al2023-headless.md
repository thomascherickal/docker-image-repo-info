## `amazoncorretto:17-al2023-headless`

```console
$ docker pull amazoncorretto@sha256:2540a0e750daaa2e72968957d88528395d2150e5b175b6909d7729962968c05c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-al2023-headless` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:6811c2c9a3cda23fae59aea381bfd04718febebe85ff505a6364b3e66370c018
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134802201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a58aaa020ec06f83691f62ce45df1622e135cb4faa74a36d2b5e50834a22457e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 22 Aug 2023 20:19:35 GMT
COPY dir:c2400bc0d1a5c32eb725de8e35d10b308c821586fa71a0a3f5ba3aa5cf9bb127 in / 
# Tue, 22 Aug 2023 20:19:35 GMT
CMD ["/bin/bash"]
# Tue, 22 Aug 2023 21:31:53 GMT
ARG version=17.0.8.7-1
# Tue, 22 Aug 2023 21:31:53 GMT
ARG package_version=1
# Tue, 22 Aug 2023 21:32:31 GMT
# ARGS: package_version=1 version=17.0.8.7-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 22 Aug 2023 21:32:31 GMT
ENV LANG=C.UTF-8
# Tue, 22 Aug 2023 21:32:31 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:1e6dafe971b21b19c13aac9adec0ca5084ccd36d780a9b704ea649071d8e7bb9`  
		Last Modified: Thu, 10 Aug 2023 03:05:52 GMT  
		Size: 52.3 MB (52305790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29d03132f5305ec936db2bc8a7648be05ce0a97446c75369302333bcfd351044`  
		Last Modified: Tue, 22 Aug 2023 21:42:45 GMT  
		Size: 82.5 MB (82496411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-al2023-headless` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:43453c72288daed8a6bba26b0c950df85e0df0084d2b408aecf84d4bb1ef453f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.2 MB (133178535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcc988dc189c8926e1e2fbde08d1f39b23d717cedd5e8c8f14613fb93cdccd96`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 22 Aug 2023 19:39:35 GMT
COPY dir:92c63817c19adbcfee66efbdf593beff7587a951a074d0392645d3c4900d19b4 in / 
# Tue, 22 Aug 2023 19:39:36 GMT
CMD ["/bin/bash"]
# Tue, 22 Aug 2023 21:11:07 GMT
ARG version=17.0.8.7-1
# Tue, 22 Aug 2023 21:11:07 GMT
ARG package_version=1
# Tue, 22 Aug 2023 21:11:38 GMT
# ARGS: package_version=1 version=17.0.8.7-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 22 Aug 2023 21:11:39 GMT
ENV LANG=C.UTF-8
# Tue, 22 Aug 2023 21:11:40 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:9fbecb9d3a17a188c49f0cab3521b4c760f46722f3e0e83726ccf3f972d8acbf`  
		Last Modified: Thu, 10 Aug 2023 03:04:18 GMT  
		Size: 51.3 MB (51348140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afabd48b0c384f288e6daec57a1b31d5c468cb71c57980d277ac25d074ecfb8`  
		Last Modified: Tue, 22 Aug 2023 21:20:20 GMT  
		Size: 81.8 MB (81830395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
