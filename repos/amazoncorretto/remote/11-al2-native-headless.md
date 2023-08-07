## `amazoncorretto:11-al2-native-headless`

```console
$ docker pull amazoncorretto@sha256:ed1133b1df7dfbcb8218c5aa6f941f420bd94912e5ba1b661da86113a98690ed
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-native-headless` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:e828ed0751fbe019f51fb5726bcf7e0889ab129a6dba7cc9e73233ae0d5db70d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.9 MB (216946742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:47d024583f4011d9a492654f945a970b81a3c25b56907b5de98272d25545e794`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 19:59:12 GMT
COPY dir:a1cfeec8f9b5a4b857222f4bbc7f5fb80ef351168a5f48841d4545523a0a3e1c in / 
# Mon, 07 Aug 2023 19:59:13 GMT
CMD ["/bin/bash"]
# Mon, 07 Aug 2023 20:52:28 GMT
ARG version=11.0.20.8-1
# Mon, 07 Aug 2023 20:54:30 GMT
# ARGS: version=11.0.20.8-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.')     && rpm --import /etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2     && echo "localpkg_gpgcheck=1" >> /etc/yum.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: rsa sha1 (md5) pgp md5 OK" || exit 1     && yum install -y $(yum deplist "${CORRETO_TEMP}/${rpm}" |grep provider | grep -vE "log4j-cve|corretto" | tr -s ' ' |cut -d ' ' -f 3 );     done     && rpm -i --nodeps ${CORRETO_TEMP}/*.rpm     && popd     && (find /usr/lib/jvm/java-11-amazon-corretto.$(uname -m) -name src.zip -delete || true)     && rm -rf ${CORRETO_TEMP}     && yum clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/yum.conf
# Mon, 07 Aug 2023 20:54:31 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:54:31 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:c0184eb4a5d5dddba3605f9adcde7e4af58050e9e4ed44751e74957c2ad0f1b4`  
		Last Modified: Tue, 01 Aug 2023 21:03:56 GMT  
		Size: 62.5 MB (62467383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309c6523704583cb83bbf4e4b23e95292efecdbdb7bdbf558bafb8fe19ac190f`  
		Last Modified: Mon, 07 Aug 2023 21:06:02 GMT  
		Size: 154.5 MB (154479359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-native-headless` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:6c4fbb19fd5b048a680d80fa6f0cc0dfced0bf0ac3f6b120d9935225d9205efa
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **210.7 MB (210681008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f77df91310f978078760bd89623c29f3dd639dec0dcbe41ae831b339106b5185`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 19:40:56 GMT
COPY dir:95dabd7a234aac70a826a1e3c0eafa3928b0be72717af1dea469f66b7db891d5 in / 
# Mon, 07 Aug 2023 19:40:57 GMT
CMD ["/bin/bash"]
# Mon, 07 Aug 2023 20:23:42 GMT
ARG version=11.0.20.8-1
# Mon, 07 Aug 2023 20:25:35 GMT
# ARGS: version=11.0.20.8-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.')     && rpm --import /etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2     && echo "localpkg_gpgcheck=1" >> /etc/yum.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-11-amazon-corretto-headless-$version.amzn2.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: rsa sha1 (md5) pgp md5 OK" || exit 1     && yum install -y $(yum deplist "${CORRETO_TEMP}/${rpm}" |grep provider | grep -vE "log4j-cve|corretto" | tr -s ' ' |cut -d ' ' -f 3 );     done     && rpm -i --nodeps ${CORRETO_TEMP}/*.rpm     && popd     && (find /usr/lib/jvm/java-11-amazon-corretto.$(uname -m) -name src.zip -delete || true)     && rm -rf ${CORRETO_TEMP}     && yum clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/yum.conf
# Mon, 07 Aug 2023 20:25:37 GMT
ENV LANG=C.UTF-8
# Mon, 07 Aug 2023 20:25:37 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:c3b5a1e75067e9d540ad8d844cad5a291a8cce89e1a3ed8e0f362a5736d3030c`  
		Last Modified: Wed, 02 Aug 2023 19:26:38 GMT  
		Size: 64.1 MB (64129548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab16d0932041effa9dbaf8956088f11e6b3ee599383224be8a673bd966d1772`  
		Last Modified: Mon, 07 Aug 2023 20:38:38 GMT  
		Size: 146.6 MB (146551460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
