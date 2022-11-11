## `amazoncorretto:17-al2022-RC-headful`

```console
$ docker pull amazoncorretto@sha256:f95b349bd237bee3c45ed539c95f93c9b6c3e89252920afead83114ca814c3f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-al2022-RC-headful` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:ebe49230e1b03f82a30a8598dc025a55647f49942b987ed3455072472b53be7b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.1 MB (137130455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec0d4edab68591f157076ac464c4738781f7248fc0b6bfe0c713489fd6edd2cd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Nov 2022 23:11:26 GMT
ADD file:541cbb916857290067c17f8f5718a02004fa3ade45da9cd68db6a3fbec9191a6 in / 
# Tue, 01 Nov 2022 23:11:26 GMT
CMD ["/bin/bash"]
# Fri, 11 Nov 2022 01:39:23 GMT
ARG version=17.0.5.8-1
# Fri, 11 Nov 2022 01:39:23 GMT
ARG package_version=1
# Fri, 11 Nov 2022 01:39:59 GMT
# ARGS: package_version=1 version=17.0.5.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2022     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2022.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 11 Nov 2022 01:39:59 GMT
ENV LANG=C.UTF-8
# Fri, 11 Nov 2022 01:39:59 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:b1f61030557f6b1b4adb79deb32494aecd38af05ed90a5d54900eea80eedc3bb`  
		Last Modified: Tue, 01 Nov 2022 23:12:19 GMT  
		Size: 57.7 MB (57657867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1df04607be2835ea2cc5d105df890bdc2e024011f143581578771fec96cbb325`  
		Last Modified: Fri, 11 Nov 2022 01:44:42 GMT  
		Size: 79.5 MB (79472588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
