## `amazoncorretto:17-al2023-RC-headful`

```console
$ docker pull amazoncorretto@sha256:ec49380849cd3281a0139b182e7c432c6398cabba6d4b19c7e50a7c5e8c78e9f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-al2023-RC-headful` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:2e2255706d8928b45ad4d277ff35bdcea3b9a3c2a34e7c120f4016c3ca0c02f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.2 MB (135228949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05328c9c5fe4245cf109d27eb61d32f1c337451fc46c29c88e3785e4be5cad33`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 15 Mar 2023 23:27:36 GMT
COPY dir:42fc532f6972d7f1219ad34006b64c07b3ddb71b58ff263ab8c6aa98dab00541 in / 
# Wed, 15 Mar 2023 23:27:37 GMT
CMD ["/bin/bash"]
# Fri, 24 Mar 2023 23:21:18 GMT
ARG version=17.0.6.10-1
# Fri, 24 Mar 2023 23:21:18 GMT
ARG package_version=1
# Fri, 24 Mar 2023 23:22:08 GMT
# ARGS: package_version=1 version=17.0.6.10-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 24 Mar 2023 23:22:08 GMT
ENV LANG=C.UTF-8
# Fri, 24 Mar 2023 23:22:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:b76f3b09316a1df6bfea69401870e8b9b4b467d535795e2ba0908c4d3bd438b9`  
		Last Modified: Wed, 15 Mar 2023 23:27:59 GMT  
		Size: 52.3 MB (52268492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4343edf01f50e0db749f2b7cb40c6188796e91243814fbc36a29da0349d32ac`  
		Last Modified: Fri, 24 Mar 2023 23:26:12 GMT  
		Size: 83.0 MB (82960457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-al2023-RC-headful` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d6889fdc83148a04623c92483128d9973683b68951f1642fe23178976648fdc1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133582741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452f5c2c94901b94c0c549344725bfa959eb717b1042a62ddf5c816c11c1d254`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 15 Mar 2023 23:39:28 GMT
COPY dir:6216321324f425942c20403c2b329b848d15da8e81fc7ff80ef8243170c71d61 in / 
# Wed, 15 Mar 2023 23:39:29 GMT
CMD ["/bin/bash"]
# Fri, 24 Mar 2023 22:45:49 GMT
ARG version=17.0.6.10-1
# Fri, 24 Mar 2023 22:45:49 GMT
ARG package_version=1
# Fri, 24 Mar 2023 22:46:33 GMT
# ARGS: package_version=1 version=17.0.6.10-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-17-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 24 Mar 2023 22:46:34 GMT
ENV LANG=C.UTF-8
# Fri, 24 Mar 2023 22:46:34 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:7ec7ca6df11f626205137bf1acf9efe68492ded671bc9f023577533727044ff6`  
		Last Modified: Wed, 15 Mar 2023 23:39:46 GMT  
		Size: 51.3 MB (51302659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00aaaef8f8101f3b45797c80ef2988d621012c1513061c5a2131d115e7fee43`  
		Last Modified: Fri, 24 Mar 2023 22:49:00 GMT  
		Size: 82.3 MB (82280082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
