## `amazoncorretto:11-al2023-headful`

```console
$ docker pull amazoncorretto@sha256:b683449f437cfc77205800b98e127f76baf4cabf53564dbfd75bdaa698dd1d72
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2023-headful` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:274798e208a8c5a136000ed68065a703486313bd8bfe6336027c0fad11301fca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.2 MB (129158070 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdac882bd314268d69f86a0d05d035d776c163cfc27c4bf39525458cbac085f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Oct 2023 01:19:32 GMT
COPY dir:9af41cf6ce642147a5bc5b6f2e8b2df0656b169c3bf33f1a1298ad1ff250d756 in / 
# Wed, 25 Oct 2023 01:19:33 GMT
CMD ["/bin/bash"]
# Wed, 25 Oct 2023 01:40:02 GMT
ARG version=11.0.21.9-1
# Wed, 25 Oct 2023 01:43:13 GMT
# ARGS: version=11.0.21.9-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm" "java-11-amazon-corretto-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Wed, 25 Oct 2023 01:43:13 GMT
ENV LANG=C.UTF-8
# Wed, 25 Oct 2023 01:43:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:e3e7439f4f2df32dd5fd7f5b3d13a3b40e7d4a7e355827d2a2e794717b58e1a0`  
		Last Modified: Tue, 24 Oct 2023 18:05:52 GMT  
		Size: 52.4 MB (52401965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1283d7898bda0a30c0f07156f35033f14af43ece3808559fd8c0acee82cff8b`  
		Last Modified: Wed, 25 Oct 2023 01:55:43 GMT  
		Size: 76.8 MB (76756105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2023-headful` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:7f152669ccf2450e2f1ed47cf80c597a76c4dd895d6aabaffd6eebece6497a13
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.4 MB (127404864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a459acfcfff58972c6b429f8ff82fa2fcba77031426dc78de37fa729ebc2feab`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Oct 2023 00:39:28 GMT
COPY dir:479ee478c40efe0225a7bfb57784564c52845a04479c6b1813627da25975830a in / 
# Wed, 25 Oct 2023 00:39:29 GMT
CMD ["/bin/bash"]
# Wed, 25 Oct 2023 01:19:37 GMT
ARG version=11.0.21.9-1
# Wed, 25 Oct 2023 01:20:30 GMT
# ARGS: version=11.0.21.9-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2023.$(uname -m).rpm" "java-11-amazon-corretto-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-11-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Wed, 25 Oct 2023 01:20:30 GMT
ENV LANG=C.UTF-8
# Wed, 25 Oct 2023 01:20:31 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:5d5c8b11ebace3512444acd4525be845e8ec3d2fd0e5999e358a7c7c74805db5`  
		Last Modified: Wed, 25 Oct 2023 00:40:02 GMT  
		Size: 51.5 MB (51479162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75247a84685f21c90c78e3c8f194cd20b992584d599e78e8dc36768462a0b98`  
		Last Modified: Wed, 25 Oct 2023 01:30:21 GMT  
		Size: 75.9 MB (75925702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
