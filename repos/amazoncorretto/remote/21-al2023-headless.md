## `amazoncorretto:21-al2023-headless`

```console
$ docker pull amazoncorretto@sha256:af374700216f3628c0ef3cb74eb576834391f59a56f3bc4febc1ae4305c0abcc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:21-al2023-headless` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:102bf9c03e1b75dd1b0b6e1bcedf595163b24d1ea7d9d0d7af6cd5f04aa442db
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.8 MB (141818976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9080e1cb9d8071071f3e296d6ae1475b28eb1a1b74fe1338664c9e6f5b454a33`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Oct 2023 01:19:32 GMT
COPY dir:9af41cf6ce642147a5bc5b6f2e8b2df0656b169c3bf33f1a1298ad1ff250d756 in / 
# Wed, 25 Oct 2023 01:19:33 GMT
CMD ["/bin/bash"]
# Wed, 25 Oct 2023 01:49:20 GMT
ARG version=21.0.1.12-1
# Thu, 02 Nov 2023 22:22:13 GMT
ARG package_version=2
# Thu, 02 Nov 2023 22:22:57 GMT
# ARGS: package_version=2 version=21.0.1.12-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-21-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-21-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Thu, 02 Nov 2023 22:22:58 GMT
ENV LANG=C.UTF-8
# Thu, 02 Nov 2023 22:22:58 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
```

-	Layers:
	-	`sha256:e3e7439f4f2df32dd5fd7f5b3d13a3b40e7d4a7e355827d2a2e794717b58e1a0`  
		Last Modified: Tue, 24 Oct 2023 18:05:52 GMT  
		Size: 52.4 MB (52401965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b95efd1914461604c3cc97570be4e4d2a86dcd45d0174ea26a01451e95c940`  
		Last Modified: Thu, 02 Nov 2023 22:26:34 GMT  
		Size: 89.4 MB (89417011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:21-al2023-headless` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:0352d59a44b54087ffb5ac94beb9ebced6d2c7be74dbf5735a815b1c561de6f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.0 MB (139972797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8afc834d79ea1427dddf79e61946a16c9f69deb9503371fb7d103df2b05b76b0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Oct 2023 00:39:28 GMT
COPY dir:479ee478c40efe0225a7bfb57784564c52845a04479c6b1813627da25975830a in / 
# Wed, 25 Oct 2023 00:39:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Oct 2023 01:25:11 GMT
ARG version=21.0.1.12-1
# Thu, 02 Nov 2023 22:40:14 GMT
ARG package_version=2
# Thu, 02 Nov 2023 22:40:56 GMT
# ARGS: package_version=2 version=21.0.1.12-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-21-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-21-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Thu, 02 Nov 2023 22:40:57 GMT
ENV LANG=C.UTF-8
# Thu, 02 Nov 2023 22:40:58 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
```

-	Layers:
	-	`sha256:5d5c8b11ebace3512444acd4525be845e8ec3d2fd0e5999e358a7c7c74805db5`  
		Last Modified: Wed, 25 Oct 2023 00:40:02 GMT  
		Size: 51.5 MB (51479162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22aad10dfd1fb0449332bf5d864ec2b8a9a36d1943e4815a176a71999d968c36`  
		Last Modified: Thu, 02 Nov 2023 22:44:11 GMT  
		Size: 88.5 MB (88493635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
