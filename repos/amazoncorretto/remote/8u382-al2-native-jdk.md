## `amazoncorretto:8u382-al2-native-jdk`

```console
$ docker pull amazoncorretto@sha256:9847ed935b57914f3a4fa1abd65ab116726ae29f0e12be7197deb4af909fd08f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u382-al2-native-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:63635fa65c991de73487a36f1e7ff6ff5726e2bcbc725d16c3b1af836c120379
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **187.8 MB (187826221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4c0733785047bcbd3bdaa1bbb9e596642140474abe1957fedab54131d32c978`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 22 Aug 2023 20:19:52 GMT
COPY dir:74433340f66bb20aa9bebf7ee91eaada91d987f210fbb253d98f2ee60012726f in / 
# Tue, 22 Aug 2023 20:19:52 GMT
CMD ["/bin/bash"]
# Tue, 22 Aug 2023 21:25:20 GMT
ARG version=1.8.0_382.b05-1
# Tue, 22 Aug 2023 21:27:48 GMT
# ARGS: version=1.8.0_382.b05-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.' | tr '_' '.'| tr -d "b" | awk -F. '{print $2"."$4"."$5"."$6}')     && rpm --import /etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2     && echo "localpkg_gpgcheck=1" >> /etc/yum.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-1.8.0-amazon-corretto-$version.amzn2.$(uname -m).rpm" "java-1.8.0-amazon-corretto-devel-$version.amzn2.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: rsa sha1 (md5) pgp md5 OK" || exit 1     && yum install -y $(yum deplist "${CORRETO_TEMP}/${rpm}" |grep provider | grep -v log4j-cve | tr -s ' ' |cut -d ' ' -f 3 );     done     && rpm -i --nodeps ${CORRETO_TEMP}/*.rpm     && popd     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto.$(uname -m) -name "*src.zip" -delete || true)     && rm -rf ${CORRETO_TEMP}     && yum clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/yum.conf
# Tue, 22 Aug 2023 21:27:49 GMT
ENV LANG=C.UTF-8
# Tue, 22 Aug 2023 21:27:49 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:8cd2389cb7276ab6d8d1154ee827bc715858f6827bdde1e9b5499a2eb3b76dc4`  
		Last Modified: Wed, 16 Aug 2023 14:05:30 GMT  
		Size: 62.5 MB (62492616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc192e4bb8c6f473b646b45107d5164177540aa9e2ad50f9dc8c950cbb828df`  
		Last Modified: Tue, 22 Aug 2023 21:39:08 GMT  
		Size: 125.3 MB (125333605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u382-al2-native-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:4e56d1ea0aa5ba75da8a5225c31ea41d9367b90cbe6d30b2bb86b867aec1ff24
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.6 MB (131582163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a45cc059e5a9c3bbec2b3e53a8f1f5e5c22e20209dffe63767aac70baffa7e41`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 22 Aug 2023 19:39:53 GMT
COPY dir:e20aef745ed6033815440b78b98680b9989b365a1e5e12e6f94169e6de7e94c3 in / 
# Tue, 22 Aug 2023 19:39:54 GMT
CMD ["/bin/bash"]
# Tue, 22 Aug 2023 21:06:27 GMT
ARG version=1.8.0_382.b05-1
# Tue, 22 Aug 2023 21:07:52 GMT
# ARGS: version=1.8.0_382.b05-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.' | tr '_' '.'| tr -d "b" | awk -F. '{print $2"."$4"."$5"."$6}')     && rpm --import /etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2     && echo "localpkg_gpgcheck=1" >> /etc/yum.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-1.8.0-amazon-corretto-$version.amzn2.$(uname -m).rpm" "java-1.8.0-amazon-corretto-devel-$version.amzn2.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: rsa sha1 (md5) pgp md5 OK" || exit 1     && yum install -y $(yum deplist "${CORRETO_TEMP}/${rpm}" |grep provider | grep -v log4j-cve | tr -s ' ' |cut -d ' ' -f 3 );     done     && rpm -i --nodeps ${CORRETO_TEMP}/*.rpm     && popd     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto.$(uname -m) -name "*src.zip" -delete || true)     && rm -rf ${CORRETO_TEMP}     && yum clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/yum.conf
# Tue, 22 Aug 2023 21:07:53 GMT
ENV LANG=C.UTF-8
# Tue, 22 Aug 2023 21:07:53 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:3e86c88b00180fc8094116a7111cfe1c0e88e04a6c513618fbde52ee5d97a51a`  
		Last Modified: Wed, 16 Aug 2023 18:15:18 GMT  
		Size: 64.1 MB (64127623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8449897f1f42b5213f010838527a0df631e66e82612fc2dab896ee260ae3a17a`  
		Last Modified: Tue, 22 Aug 2023 21:16:44 GMT  
		Size: 67.5 MB (67454540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
