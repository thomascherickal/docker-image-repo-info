## `amazoncorretto:11-al2022-RC-headful`

```console
$ docker pull amazoncorretto@sha256:14282b0d63cee97243d561899f52c57b82dbd78f324d9fce546bb9af3be65b2f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:11-al2022-RC-headful` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:a71c9df6aed791463ee4b9429bb8a9bd4ffd3d95ffad7fc2db9a074a875d6520
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.8 MB (132833209 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b246ae6f34ac404296b798c22143b4b8e5324f1d9f149a2786daa757d487bebc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Nov 2022 23:11:26 GMT
ADD file:541cbb916857290067c17f8f5718a02004fa3ade45da9cd68db6a3fbec9191a6 in / 
# Tue, 01 Nov 2022 23:11:26 GMT
CMD ["/bin/bash"]
# Fri, 11 Nov 2022 01:38:06 GMT
ARG version=11.0.17.8-1
# Fri, 11 Nov 2022 01:39:06 GMT
# ARGS: version=11.0.17.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2022     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2022.$(uname -m).rpm" "java-11-amazon-corretto-$version.amzn2022.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 11 Nov 2022 01:39:06 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:39:06 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:b1f61030557f6b1b4adb79deb32494aecd38af05ed90a5d54900eea80eedc3bb`  
		Last Modified: Tue, 01 Nov 2022 23:12:19 GMT  
		Size: 57.7 MB (57657867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b3e19463f7f76dd6501192b2b9b43f74f15ff205d3eb4a82c004014aa1ca681`  
		Last Modified: Fri, 11 Nov 2022 01:43:52 GMT  
		Size: 75.2 MB (75175342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
