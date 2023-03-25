## `amazoncorretto:11-al2023-RC-headful`

```console
$ docker pull amazoncorretto@sha256:ad939d5299118d92c6cddabb4706234b683852eab9cadf2fa919424973a4080c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2023-RC-headful` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:88c5e5e4c3fb6684742d052cbca5bd0e1f1ec9cbcb27a1fc7285928939a59a09
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.8 MB (128789999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a68b822715b489f62c2f986b43ba188cfd6a57354f196cc33be37f4247a41fc`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 15 Mar 2023 23:27:36 GMT
COPY dir:42fc532f6972d7f1219ad34006b64c07b3ddb71b58ff263ab8c6aa98dab00541 in / 
# Wed, 15 Mar 2023 23:27:37 GMT
CMD ["/bin/bash"]
# Fri, 24 Mar 2023 23:20:20 GMT
ARG version=11.0.18.10-1
# Fri, 24 Mar 2023 23:21:07 GMT
# ARGS: version=11.0.18.10-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm" "java-11-amazon-corretto-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 24 Mar 2023 23:21:07 GMT
ENV LANG=C.UTF-8
# Fri, 24 Mar 2023 23:21:07 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:b76f3b09316a1df6bfea69401870e8b9b4b467d535795e2ba0908c4d3bd438b9`  
		Last Modified: Wed, 15 Mar 2023 23:27:59 GMT  
		Size: 52.3 MB (52268492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d789698b37e7f9347119f428361ace6b29220f6dfe9a3a330828e1112208d24`  
		Last Modified: Fri, 24 Mar 2023 23:25:07 GMT  
		Size: 76.5 MB (76521507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2023-RC-headful` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:69e09e4a6223df4553aa52b2c4f72e5a18fc512be7bd41ccc6cdbe158b8b6ef8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (126986577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c14acbcb8a2575cb6436835d401b93cc5b7e2816076529be602e37d46bd191f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 15 Mar 2023 23:39:28 GMT
COPY dir:6216321324f425942c20403c2b329b848d15da8e81fc7ff80ef8243170c71d61 in / 
# Wed, 15 Mar 2023 23:39:29 GMT
CMD ["/bin/bash"]
# Fri, 24 Mar 2023 22:45:00 GMT
ARG version=11.0.18.10-1
# Fri, 24 Mar 2023 22:45:44 GMT
# ARGS: version=11.0.18.10-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm" "java-11-amazon-corretto-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 24 Mar 2023 22:45:45 GMT
ENV LANG=C.UTF-8
# Fri, 24 Mar 2023 22:45:45 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:7ec7ca6df11f626205137bf1acf9efe68492ded671bc9f023577533727044ff6`  
		Last Modified: Wed, 15 Mar 2023 23:39:46 GMT  
		Size: 51.3 MB (51302659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb4c3013cd4410afc2d97daec38512be1a69f7434c7f1cf89629931a23cba39`  
		Last Modified: Fri, 24 Mar 2023 22:48:07 GMT  
		Size: 75.7 MB (75683918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
