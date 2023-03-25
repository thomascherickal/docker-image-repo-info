## `amazoncorretto:8-al2023-RC-jre`

```console
$ docker pull amazoncorretto@sha256:5269789c06750a09fc607173dc6b2ea43e2b95c3956462cedf43aeb2584a8a39
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8-al2023-RC-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:617d850ce0df2a5ede84fef6878cd4ac402d74d7d2e5c66361735724e68ec3ee
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.6 MB (330584617 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f3c0e5a28881afa28e544856da5916467a405078076b1ec60e90838252df8a1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 15 Mar 2023 23:27:36 GMT
COPY dir:42fc532f6972d7f1219ad34006b64c07b3ddb71b58ff263ab8c6aa98dab00541 in / 
# Wed, 15 Mar 2023 23:27:37 GMT
CMD ["/bin/bash"]
# Fri, 24 Mar 2023 23:19:26 GMT
ARG version=1.8.0_362.b08-1
# Fri, 24 Mar 2023 23:19:59 GMT
# ARGS: version=1.8.0_362.b08-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.' | tr '_' '.'| tr -d "b" | awk -F. '{print $2"."$4"."$5"."$6}')     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-1.8.0-amazon-corretto-$version.amzn2023.$(uname -m).rpm" "java-1.8.0-amazon-corretto-devel-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-1.8.0-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 24 Mar 2023 23:20:01 GMT
ENV LANG=C.UTF-8
# Fri, 24 Mar 2023 23:20:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:b76f3b09316a1df6bfea69401870e8b9b4b467d535795e2ba0908c4d3bd438b9`  
		Last Modified: Wed, 15 Mar 2023 23:27:59 GMT  
		Size: 52.3 MB (52268492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b00a676396ba418ec7ec8fa8f0e5fb83b262592a68c2f6411ad0b33412b2f5`  
		Last Modified: Fri, 24 Mar 2023 23:23:57 GMT  
		Size: 278.3 MB (278316125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8-al2023-RC-jre` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:49b6b8f5dee4efa77220e99b0c4a700d667b7137a810ecdc4afac9c2694c3340
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.8 MB (169812892 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:603b5ee7b9eeace86c39269793ea72a39e8cb3ca9de4c92ec9b05f580dba7d26`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 15 Mar 2023 23:39:28 GMT
COPY dir:6216321324f425942c20403c2b329b848d15da8e81fc7ff80ef8243170c71d61 in / 
# Wed, 15 Mar 2023 23:39:29 GMT
CMD ["/bin/bash"]
# Fri, 24 Mar 2023 22:44:40 GMT
ARG version=1.8.0_362.b08-1
# Fri, 24 Mar 2023 22:44:54 GMT
# ARGS: version=1.8.0_362.b08-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.' | tr '_' '.'| tr -d "b" | awk -F. '{print $2"."$4"."$5"."$6}')     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-1.8.0-amazon-corretto-$version.amzn2023.$(uname -m).rpm" "java-1.8.0-amazon-corretto-devel-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-1.8.0-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Fri, 24 Mar 2023 22:44:55 GMT
ENV LANG=C.UTF-8
# Fri, 24 Mar 2023 22:44:55 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:7ec7ca6df11f626205137bf1acf9efe68492ded671bc9f023577533727044ff6`  
		Last Modified: Wed, 15 Mar 2023 23:39:46 GMT  
		Size: 51.3 MB (51302659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023be9f96460183720eca975758b191aa3191079a2d03521071dd67d6e899155`  
		Last Modified: Fri, 24 Mar 2023 22:47:12 GMT  
		Size: 118.5 MB (118510233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
