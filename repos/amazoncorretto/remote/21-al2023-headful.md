## `amazoncorretto:21-al2023-headful`

```console
$ docker pull amazoncorretto@sha256:8084b733f95327b906612ab5cb10a5b3ddd073657d8d02718beffbc9358b830e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:21-al2023-headful` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:29a4a6e4f7c9716f69da35def2434e9e92c85e8bc9b209db1446298ceefd1889
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.3 MB (142339736 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c79743ac6a5b5025ad0922bc191c1f43960803860224e5a74bbbe094ce8b4c48`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:21:34 GMT
COPY dir:a736dc55b3f736cb7e8fc1978dac2536c3df3a8e3e684d650ab946ec3bfffd4d in / 
# Tue, 21 Nov 2023 03:21:35 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 04:23:20 GMT
ARG version=21.0.1.12-1
# Tue, 21 Nov 2023 04:23:20 GMT
ARG package_version=2
# Tue, 21 Nov 2023 04:24:25 GMT
# ARGS: package_version=2 version=21.0.1.12-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-21-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-21-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-21-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 21 Nov 2023 04:24:25 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 04:24:25 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
```

-	Layers:
	-	`sha256:bad342ce986c7387f9e03cc2deafa306717aed86685ac6e1705ccc016b283eca`  
		Last Modified: Tue, 14 Nov 2023 20:44:05 GMT  
		Size: 52.2 MB (52218672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f861194af8f07eac3b9497691f3e4a1a105fcc8720a1ff5b110abf2c64d76d0f`  
		Last Modified: Tue, 21 Nov 2023 04:34:00 GMT  
		Size: 90.1 MB (90121064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:21-al2023-headful` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:427ba879aae029f8cb2108c276855efbd7aeb371142a5a7029079c2cfb54875a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.5 MB (140517558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b0845f813566f11011ac85156e2ea6ba08c01ec50f7229e1275f8ffb89c38ad`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:39:34 GMT
COPY dir:fac986ebd66714776e9e2c25ed83431bd5e6692d32fdb5c2c74b9c2916168b3e in / 
# Tue, 21 Nov 2023 03:39:34 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 05:14:46 GMT
ARG version=21.0.1.12-1
# Tue, 21 Nov 2023 05:14:46 GMT
ARG package_version=2
# Tue, 21 Nov 2023 05:15:39 GMT
# ARGS: package_version=2 version=21.0.1.12-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-21-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-21-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-21-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 21 Nov 2023 05:15:40 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 05:15:40 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
```

-	Layers:
	-	`sha256:f8ec7f6a4acb7febbe0e77fe9bba1064900d89cbf939e87733102926ad5870fd`  
		Last Modified: Tue, 14 Nov 2023 20:44:04 GMT  
		Size: 51.3 MB (51307015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9107b54845c376000fa7b20619ac7838d8a0fa057744f12a9b3c4dd21d18a5dc`  
		Last Modified: Tue, 21 Nov 2023 05:24:12 GMT  
		Size: 89.2 MB (89210543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
