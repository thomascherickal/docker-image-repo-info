## `amazoncorretto:11-al2-native-headless`

```console
$ docker pull amazoncorretto@sha256:a3c251a1833ac4d8f7aa1ef8345c16d5eacbdcf9f47f74a80dc7a8d47b13ae32
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-native-headless` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:26a29dd2cfb240798d0da45c0df3929ddf10b619b4c9670e03de591c849da122
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.0 MB (217023263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ccbe1a587fcbdf7d86377282635285ce1d12275800eb0fef42083945fa3da60`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 22 Aug 2023 20:19:52 GMT
COPY dir:74433340f66bb20aa9bebf7ee91eaada91d987f210fbb253d98f2ee60012726f in / 
# Tue, 22 Aug 2023 20:19:52 GMT
CMD ["/bin/bash"]
# Tue, 22 Aug 2023 21:28:14 GMT
ARG version=11.0.20.8-1
# Tue, 22 Aug 2023 21:30:22 GMT
# ARGS: version=11.0.20.8-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.')     && rpm --import /etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2     && echo "localpkg_gpgcheck=1" >> /etc/yum.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: rsa sha1 (md5) pgp md5 OK" || exit 1     && yum install -y $(yum deplist "${CORRETO_TEMP}/${rpm}" |grep provider | grep -vE "log4j-cve|corretto" | tr -s ' ' |cut -d ' ' -f 3 );     done     && rpm -i --nodeps ${CORRETO_TEMP}/*.rpm     && popd     && (find /usr/lib/jvm/java-11-amazon-corretto.$(uname -m) -name src.zip -delete || true)     && rm -rf ${CORRETO_TEMP}     && yum clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/yum.conf
# Tue, 22 Aug 2023 21:30:23 GMT
ENV LANG=C.UTF-8
# Tue, 22 Aug 2023 21:30:23 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:8cd2389cb7276ab6d8d1154ee827bc715858f6827bdde1e9b5499a2eb3b76dc4`  
		Last Modified: Wed, 16 Aug 2023 14:05:30 GMT  
		Size: 62.5 MB (62492616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:725436ce503d8ad728c8f4f1834a2358a1dbc5d066acbc946531504813918717`  
		Last Modified: Tue, 22 Aug 2023 21:41:08 GMT  
		Size: 154.5 MB (154530647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-native-headless` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:30aa3f2df540a1b73ea670c51507b6d381a2f5854e0ae5ae5617c8c15d7ed7ec
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.7 MB (210678982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56dca8eae10da0ac45e47eed75ea76dbb24712a8d4854ddea50697b1d3bb26f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 22 Aug 2023 19:39:53 GMT
COPY dir:e20aef745ed6033815440b78b98680b9989b365a1e5e12e6f94169e6de7e94c3 in / 
# Tue, 22 Aug 2023 19:39:54 GMT
CMD ["/bin/bash"]
# Tue, 22 Aug 2023 21:08:10 GMT
ARG version=11.0.20.8-1
# Tue, 22 Aug 2023 21:09:56 GMT
# ARGS: version=11.0.20.8-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.')     && rpm --import /etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2     && echo "localpkg_gpgcheck=1" >> /etc/yum.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: rsa sha1 (md5) pgp md5 OK" || exit 1     && yum install -y $(yum deplist "${CORRETO_TEMP}/${rpm}" |grep provider | grep -vE "log4j-cve|corretto" | tr -s ' ' |cut -d ' ' -f 3 );     done     && rpm -i --nodeps ${CORRETO_TEMP}/*.rpm     && popd     && (find /usr/lib/jvm/java-11-amazon-corretto.$(uname -m) -name src.zip -delete || true)     && rm -rf ${CORRETO_TEMP}     && yum clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/yum.conf
# Tue, 22 Aug 2023 21:09:58 GMT
ENV LANG=C.UTF-8
# Tue, 22 Aug 2023 21:09:58 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:3e86c88b00180fc8094116a7111cfe1c0e88e04a6c513618fbde52ee5d97a51a`  
		Last Modified: Wed, 16 Aug 2023 18:15:18 GMT  
		Size: 64.1 MB (64127623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9269b0a1ed7c3a42af347c4a4d67bfb8720c080c5f2a33bf8c2a929ffa695f97`  
		Last Modified: Tue, 22 Aug 2023 21:18:34 GMT  
		Size: 146.6 MB (146551359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
