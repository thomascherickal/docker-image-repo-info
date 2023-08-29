## `maven:3-amazoncorretto-8-al2023`

```console
$ docker pull maven@sha256:590fecb27e1d76d8d44c005782773bb244bc8533a1053696da3773e8c85bf6f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-8-al2023` - linux; amd64

```console
$ docker pull maven@sha256:f6f89a6abe9019285a97d0fa6d5392eb076d0622440834da458e7b764a827e90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **378.3 MB (378328885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3cb87455c26bead0c45e70dfe6ef7e1de4052f7629959bd4455dfc7d237b644`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 29 Aug 2023 18:29:04 GMT
COPY dir:5aeab1edfeaa7561058aadd3dc752f2959c8cd0e5442b979406e3948fdedb852 in / 
# Tue, 29 Aug 2023 18:29:05 GMT
CMD ["/bin/bash"]
# Tue, 29 Aug 2023 19:39:27 GMT
ARG version=1.8.0_382.b05-1
# Tue, 29 Aug 2023 19:40:01 GMT
# ARGS: version=1.8.0_382.b05-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.' | tr '_' '.'| tr -d "b" | awk -F. '{print $2"."$4"."$5"."$6}')     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-1.8.0-amazon-corretto-$version.amzn2023.$(uname -m).rpm" "java-1.8.0-amazon-corretto-devel-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-1.8.0-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 29 Aug 2023 19:40:03 GMT
ENV LANG=C.UTF-8
# Tue, 29 Aug 2023 19:40:03 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Mon, 28 Aug 2023 11:26:15 GMT
RUN yum install -y tar which gzip findutils # TODO remove # buildkit
# Mon, 28 Aug 2023 11:26:15 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 28 Aug 2023 11:26:15 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Mon, 28 Aug 2023 11:26:15 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Mon, 28 Aug 2023 11:26:15 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Mon, 28 Aug 2023 11:26:15 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Mon, 28 Aug 2023 11:26:15 GMT
ARG MAVEN_VERSION=3.9.4
# Mon, 28 Aug 2023 11:26:15 GMT
ARG USER_HOME_DIR=/root
# Mon, 28 Aug 2023 11:26:15 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 28 Aug 2023 11:26:15 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 28 Aug 2023 11:26:15 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:8c169abda7fcf89d4baeaacf8e5d709a6112b4a6babe0c195a42404bca597f55`  
		Last Modified: Sat, 26 Aug 2023 03:05:59 GMT  
		Size: 52.3 MB (52287844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec251684f638aedaeec62729cbd1f0ff8d45152c11aaf6d80206b80a23793dd`  
		Last Modified: Tue, 29 Aug 2023 19:52:50 GMT  
		Size: 278.4 MB (278414461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26d0344dee114f3c605c8557c13c21ff2ad1a27a6a8f91a2518c0854584b168`  
		Last Modified: Tue, 29 Aug 2023 20:21:34 GMT  
		Size: 38.2 MB (38218793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a064dbada395ce5d77629990718241a5bc77ec6f0995359c655eb4785d55769c`  
		Last Modified: Tue, 29 Aug 2023 20:21:32 GMT  
		Size: 9.4 MB (9406407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87bdbc4d370c07d88ae637fe37b4a825a90bf3dd38be66e2c0aaef7b41dbbf5`  
		Last Modified: Tue, 29 Aug 2023 20:21:31 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b49a621142fbf4bea8b1bd5cc23b3632349665803f7a34ba4ccdd6f65c40b8f`  
		Last Modified: Tue, 29 Aug 2023 20:21:31 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:172cf0397e5fd9759f1ef21619ee4a0ad1558d97e3bd14a83f63ad8fa5a35276`  
		Last Modified: Tue, 29 Aug 2023 20:21:31 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-8-al2023` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:6cb52dfbc91cab9bdf51cb5df6f0369c773afdedaa8e7c28ce11488a1cf00dda
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.7 MB (215694287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:570d2fb19c946848efcacf4204c7317470f5ba4ae7361f0b1f0c7198b0970f6c`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 29 Aug 2023 18:40:45 GMT
COPY dir:0004a2667b3e5dc5080ba46954457d05835caf07f7030d94b953f1c3cede9b0c in / 
# Tue, 29 Aug 2023 18:40:47 GMT
CMD ["/bin/bash"]
# Tue, 29 Aug 2023 19:06:45 GMT
ARG version=1.8.0_382.b05-1
# Tue, 29 Aug 2023 19:07:01 GMT
# ARGS: version=1.8.0_382.b05-1
RUN set -eux     && export resouce_version=$(echo $version | tr '-' '.' | tr '_' '.'| tr -d "b" | awk -F. '{print $2"."$4"."$5"."$6}')     && rpm --import file:///etc/pki/rpm-gpg/RPM-GPG-KEY-amazon-linux-2023     && echo "localpkg_gpgcheck=1" >> /etc/dnf/dnf.conf     && CORRETO_TEMP=$(mktemp -d)     && pushd ${CORRETO_TEMP}     && RPM_LIST=("java-1.8.0-amazon-corretto-$version.amzn2023.$(uname -m).rpm" "java-1.8.0-amazon-corretto-devel-$version.amzn2023.$(uname -m).rpm")     && for rpm in ${RPM_LIST[@]}; do     curl --fail -O https://corretto.aws/downloads/resources/${resouce_version}/${rpm}     && rpm -K "${CORRETO_TEMP}/${rpm}" | grep -F "${CORRETO_TEMP}/${rpm}: digests signatures OK" || exit 1;     done     && dnf install -y ${CORRETO_TEMP}/*.rpm     && popd     && rm -rf /usr/lib/jvm/java-1.8.0-amazon-corretto.$(uname -m)/lib/src.zip     && rm -rf ${CORRETO_TEMP}     && dnf clean all     && rm -rf /var/cache/yum     && sed -i '/localpkg_gpgcheck=1/d' /etc/dnf/dnf.conf
# Tue, 29 Aug 2023 19:07:02 GMT
ENV LANG=C.UTF-8
# Tue, 29 Aug 2023 19:07:02 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Mon, 28 Aug 2023 11:26:15 GMT
RUN yum install -y tar which gzip findutils # TODO remove # buildkit
# Mon, 28 Aug 2023 11:26:15 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 28 Aug 2023 11:26:15 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Mon, 28 Aug 2023 11:26:15 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Mon, 28 Aug 2023 11:26:15 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Mon, 28 Aug 2023 11:26:15 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Mon, 28 Aug 2023 11:26:15 GMT
ARG MAVEN_VERSION=3.9.4
# Mon, 28 Aug 2023 11:26:15 GMT
ARG USER_HOME_DIR=/root
# Mon, 28 Aug 2023 11:26:15 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 28 Aug 2023 11:26:15 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 28 Aug 2023 11:26:15 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:8e2acd49419010bc77a61e38a85963f09e403f004635f24c436d177a08df1040`  
		Last Modified: Sat, 26 Aug 2023 03:06:10 GMT  
		Size: 51.3 MB (51324150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:536f74ffb0681fda3a2ef70e6e8227d98cb13428bec8b3c5398252ca678e6870`  
		Last Modified: Tue, 29 Aug 2023 19:16:49 GMT  
		Size: 118.6 MB (118574076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27e54eeb343c47b1ba04ae9afe15720fa582ca949b62dc6dc402595c67fa613`  
		Last Modified: Tue, 29 Aug 2023 19:52:59 GMT  
		Size: 36.4 MB (36388265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6f7576173aee1ca44a8d4100d54d325c65baf21a6a7b5b02d30bcb4f1a4c91`  
		Last Modified: Tue, 29 Aug 2023 19:52:58 GMT  
		Size: 9.4 MB (9406416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:056dd836a1e2e8110451560220eea8502868cdd3591d1d67b78e26458046e3ad`  
		Last Modified: Tue, 29 Aug 2023 19:52:57 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b612a9a837b1eea35bfa1772a2a3d6e2a6d6aecbf884c06775960e142b44f0b5`  
		Last Modified: Tue, 29 Aug 2023 19:52:57 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ee0f4b288aa84b0433be3e0f12c70ab5384b11ab3632edb20219fc4d4e0863`  
		Last Modified: Tue, 29 Aug 2023 19:52:57 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
