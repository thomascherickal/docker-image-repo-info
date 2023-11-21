## `amazoncorretto:17-al2023-headless`

```console
$ docker pull amazoncorretto@sha256:f3257e96275e8229da8c3f91958b97092ac6154aa379d578a880257ed767f8ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-al2023-headless` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:e862ab08efaac42dfbb437a89dfc4ae03f508fdcdde09f4210948c7e107a0e3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.5 MB (134538537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca3460524d29e0d8ad85b23b59b771fe5a7cf7f2964486a5152a7a3172d6319d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:21:34 GMT
COPY dir:a736dc55b3f736cb7e8fc1978dac2536c3df3a8e3e684d650ab946ec3bfffd4d in / 
# Tue, 21 Nov 2023 03:21:35 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 04:19:35 GMT
ARG version=17.0.9.8-1
# Tue, 21 Nov 2023 04:19:35 GMT
ARG package_version=1
# Tue, 21 Nov 2023 04:20:14 GMT
# ARGS: package_version=1 version=17.0.9.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 21 Nov 2023 04:20:14 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 04:20:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:bad342ce986c7387f9e03cc2deafa306717aed86685ac6e1705ccc016b283eca`  
		Last Modified: Tue, 14 Nov 2023 20:44:05 GMT  
		Size: 52.2 MB (52218672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83af13d88a71252212dfa43073f96ba364a183cd65bf7c464fbf735d035da892`  
		Last Modified: Tue, 21 Nov 2023 04:30:59 GMT  
		Size: 82.3 MB (82319865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-al2023-headless` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:9d4720009181b1e100e9a114ef70806da07615f57bb1b0f41246ef980d64c1ce
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.0 MB (132960448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:711cb1c7114a3beca736cc1080c6389fb6f5645f412dccc45dd9be8389caca05`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Nov 2023 03:39:34 GMT
COPY dir:fac986ebd66714776e9e2c25ed83431bd5e6692d32fdb5c2c74b9c2916168b3e in / 
# Tue, 21 Nov 2023 03:39:34 GMT
CMD ["/bin/bash"]
# Tue, 21 Nov 2023 05:11:40 GMT
ARG version=17.0.9.8-1
# Tue, 21 Nov 2023 05:11:40 GMT
ARG package_version=1
# Tue, 21 Nov 2023 05:12:17 GMT
# ARGS: package_version=1 version=17.0.9.8-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-17-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-17-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 21 Nov 2023 05:12:18 GMT
ENV LANG=C.UTF-8
# Tue, 21 Nov 2023 05:12:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:f8ec7f6a4acb7febbe0e77fe9bba1064900d89cbf939e87733102926ad5870fd`  
		Last Modified: Tue, 14 Nov 2023 20:44:04 GMT  
		Size: 51.3 MB (51307015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6ac6fa244a58155fb570a7728fe7e7e5477e62610d663398579be0c4d7f920`  
		Last Modified: Tue, 21 Nov 2023 05:21:28 GMT  
		Size: 81.7 MB (81653433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
