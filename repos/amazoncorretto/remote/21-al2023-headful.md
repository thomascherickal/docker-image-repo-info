## `amazoncorretto:21-al2023-headful`

```console
$ docker pull amazoncorretto@sha256:49b6cbdeb9302c322fe4dc067ec9c9464e2d602398c8b8369cf058923546ae2c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:21-al2023-headful` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:56768572556e34ac6e4b2e6372e60aaf64d75a8b376662ee7d5c24f2aadc3341
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.5 MB (142522657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12329c0907510bfbb5628d8c350de5bbcecc2c41e1e94732b9858d68897d3074`
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
# Thu, 02 Nov 2023 22:23:18 GMT
# ARGS: package_version=2 version=21.0.1.12-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-21-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-21-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-21-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Thu, 02 Nov 2023 22:23:18 GMT
ENV LANG=C.UTF-8
# Thu, 02 Nov 2023 22:23:18 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
```

-	Layers:
	-	`sha256:e3e7439f4f2df32dd5fd7f5b3d13a3b40e7d4a7e355827d2a2e794717b58e1a0`  
		Last Modified: Tue, 24 Oct 2023 18:05:52 GMT  
		Size: 52.4 MB (52401965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a03e93705168cb6b27edb6ed0a91e39ddd070effe4cb58dab3e5e99350ae7001`  
		Last Modified: Thu, 02 Nov 2023 22:26:54 GMT  
		Size: 90.1 MB (90120692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:21-al2023-headful` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:0a41f5a70cdb8d6c185c2e82fa18238b294dbb397d0610d2c2bd9565e338a485
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.7 MB (140687346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:81369bc93cca170de905f9c3e395ec451e5f8bde3221f0248415ccb95e59dfb9`
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
# Thu, 02 Nov 2023 22:41:16 GMT
# ARGS: package_version=2 version=21.0.1.12-1
RUN set -eux     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-21-amazon-corretto-headless-$version.amzn2023.${package_version}.$(uname -m).rpm" "java-21-amazon-corretto-$version.amzn2023.${package_version}.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/$(echo $version | tr '-' '.')/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-21-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Thu, 02 Nov 2023 22:41:17 GMT
ENV LANG=C.UTF-8
# Thu, 02 Nov 2023 22:41:17 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
```

-	Layers:
	-	`sha256:5d5c8b11ebace3512444acd4525be845e8ec3d2fd0e5999e358a7c7c74805db5`  
		Last Modified: Wed, 25 Oct 2023 00:40:02 GMT  
		Size: 51.5 MB (51479162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2072fa60895710d2b97f22ed32c0a68e8005c0279904a6e5a2211dc3486e235a`  
		Last Modified: Thu, 02 Nov 2023 22:44:29 GMT  
		Size: 89.2 MB (89208184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
