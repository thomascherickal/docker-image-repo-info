## `amazoncorretto:11-al2023-headless`

```console
$ docker pull amazoncorretto@sha256:10aa25f4d2563ef1ee4d050cc13fb35d7fa6f7c1c01581b7e47dc0b29539663d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2023-headless` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:5401538a2e5ba775f3131b26b77976ed4f76e52c048921c3fda2741f92f18e92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.3 MB (128274125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:290deb1d529fa681f71d4f79978269450fa4d89aa401f29ca6758f3fbdc9f029`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:21:34 GMT
COPY dir:a736dc55b3f736cb7e8fc1978dac2536c3df3a8e3e684d650ab946ec3bfffd4d in / 
# Tue, 21 Nov 2023 03:21:35 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 04:16:24 GMT
ARG version=11.0.21.9-1
# Tue, 21 Nov 2023 04:17:02 GMT
# ARGS: version=11.0.21.9-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 21 Nov 2023 04:17:03 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 04:17:03 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:bad342ce986c7387f9e03cc2deafa306717aed86685ac6e1705ccc016b283eca`  
		Last Modified: Tue, 14 Nov 2023 20:44:05 GMT  
		Size: 52.2 MB (52218672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6041538b106fcfd2d3106888b5fc730d8cb1788e78661c272d6b0ae8c4aa36d`  
		Last Modified: Tue, 21 Nov 2023 04:28:44 GMT  
		Size: 76.1 MB (76055453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2023-headless` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:922944b513ad1a6610d6f1d26b042ab6a7d2436b080ee14ec7915f8648073f0c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.5 MB (126537504 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b49f0ff9e6623ba9fc1e145eb71f03e02a8e6c5d41805dd34789eee12ebd6ca8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:39:34 GMT
COPY dir:fac986ebd66714776e9e2c25ed83431bd5e6692d32fdb5c2c74b9c2916168b3e in / 
# Tue, 21 Nov 2023 03:39:34 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 05:09:15 GMT
ARG version=11.0.21.9-1
# Tue, 21 Nov 2023 05:09:51 GMT
# ARGS: version=11.0.21.9-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 21 Nov 2023 05:09:52 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 05:09:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:f8ec7f6a4acb7febbe0e77fe9bba1064900d89cbf939e87733102926ad5870fd`  
		Last Modified: Tue, 14 Nov 2023 20:44:04 GMT  
		Size: 51.3 MB (51307015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e9e1614e64638a36500b7ced830823a551bfcef9977396334d414a1f683534`  
		Last Modified: Tue, 21 Nov 2023 05:19:14 GMT  
		Size: 75.2 MB (75230489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
