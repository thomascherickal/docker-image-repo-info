## `maven:3-amazoncorretto-17`

```console
$ docker pull maven@sha256:1c515e2c998b0cc717d5639c130099d9bb1bfd0f7eabcc9f041d9fad4c7e04ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-17` - linux; amd64

```console
$ docker pull maven@sha256:399cf920b33d7c0bbda16498664bddc18eca0c387a429019e96aa0c1f4cf15cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **373.3 MB (373273032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc793153dccde6d9a7a7cbe82431dd9a460e3d4c54a1d639a06f8c68415144b5`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 28 Mar 2023 18:20:51 GMT
COPY dir:d74df4759bcd6e2619baa3ec354d8703c77c836345c6a887554df76aaf1d9965 in / 
# Tue, 28 Mar 2023 18:20:52 GMT
CMD ["/bin/bash"]
# Thu, 20 Apr 2023 18:23:27 GMT
ARG version=17.0.7.7-1
# Thu, 20 Apr 2023 18:23:51 GMT
# ARGS: version=17.0.7.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 20 Apr 2023 18:23:52 GMT
ENV LANG=C.UTF-8
# Thu, 20 Apr 2023 18:23:52 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Thu, 20 Apr 2023 18:23:52 GMT
RUN yum install -y tar which gzip # TODO remove # buildkit
# Thu, 20 Apr 2023 18:23:52 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 20 Apr 2023 18:23:52 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Thu, 20 Apr 2023 18:23:52 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Thu, 20 Apr 2023 18:23:52 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Thu, 20 Apr 2023 18:23:52 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Thu, 20 Apr 2023 18:23:52 GMT
ARG MAVEN_VERSION=3.9.1
# Thu, 20 Apr 2023 18:23:52 GMT
ARG USER_HOME_DIR=/root
# Thu, 20 Apr 2023 18:23:52 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 20 Apr 2023 18:23:52 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 20 Apr 2023 18:23:52 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:128d54f2c9b134270b406c5f3a41296da7c1111d3a6927f0b4451131d636151e`  
		Last Modified: Thu, 23 Mar 2023 21:24:22 GMT  
		Size: 62.5 MB (62483466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e31014b690dd2ee54ea3b7a7bd92073be9fb2dbac3c4274c71a7e30facd6e0`  
		Last Modified: Thu, 20 Apr 2023 18:34:30 GMT  
		Size: 151.9 MB (151949564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168b6cff6a088a81df4295619fac068ab9227bec5715cf98930ba424803301dc`  
		Last Modified: Thu, 20 Apr 2023 19:09:47 GMT  
		Size: 149.7 MB (149732453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff3b7b82239c3b512971808fc98ae1e4cd145caaf90e764d48beb4a396fc336`  
		Last Modified: Thu, 20 Apr 2023 19:09:35 GMT  
		Size: 9.1 MB (9106162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a133bff6a27dd1cfddf8b00652984709803d63681a85966c5ed72abe4f29ac4`  
		Last Modified: Thu, 20 Apr 2023 19:09:34 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f400ed0320414636528d0dc6a1e4dd3482b2960b77192127206deb0e12662309`  
		Last Modified: Thu, 20 Apr 2023 19:09:34 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ced469bfad428130e08848e478a8f22ed35941ec30469ff408f7f194924b90`  
		Last Modified: Thu, 20 Apr 2023 19:09:34 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-17` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:1f4702f577961d8e2f5ce468fca6714e00794aea8eb33c4574fffcedede5c2c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **338.6 MB (338572329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e9243e6a9b66aba4aee1a7af212c661fdab5f514a85f9148da7895e120c4e86`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Tue, 28 Mar 2023 18:40:10 GMT
COPY dir:1d0df99dbb2a961dca382ec30c27f40e06635a9186a0715c0d2a629262a04288 in / 
# Tue, 28 Mar 2023 18:40:10 GMT
CMD ["/bin/bash"]
# Thu, 20 Apr 2023 17:42:46 GMT
ARG version=17.0.7.7-1
# Thu, 20 Apr 2023 17:43:06 GMT
# ARGS: version=17.0.7.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 20 Apr 2023 17:43:08 GMT
ENV LANG=C.UTF-8
# Thu, 20 Apr 2023 17:43:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
# Thu, 20 Apr 2023 17:43:08 GMT
RUN yum install -y tar which gzip # TODO remove # buildkit
# Thu, 20 Apr 2023 17:43:08 GMT
ENV MAVEN_HOME=/usr/share/maven
# Thu, 20 Apr 2023 17:43:08 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Thu, 20 Apr 2023 17:43:08 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Thu, 20 Apr 2023 17:43:08 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Thu, 20 Apr 2023 17:43:08 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Thu, 20 Apr 2023 17:43:08 GMT
ARG MAVEN_VERSION=3.9.1
# Thu, 20 Apr 2023 17:43:08 GMT
ARG USER_HOME_DIR=/root
# Thu, 20 Apr 2023 17:43:08 GMT
ENV MAVEN_CONFIG=/root/.m2
# Thu, 20 Apr 2023 17:43:08 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Thu, 20 Apr 2023 17:43:08 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:949542da27c3c0ab979766d37f455344960f838d9f661b9db50bec634ca7149e`  
		Last Modified: Thu, 23 Mar 2023 21:25:53 GMT  
		Size: 64.1 MB (64126936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d5f25839cc5d9c044ea00ba0de0880e3272fc9e31ae1d800e809913883f78b`  
		Last Modified: Thu, 20 Apr 2023 17:53:14 GMT  
		Size: 150.5 MB (150487733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156c43e9c3d8af2d90c6d0fa58cb3d644c05f7a235923991f65ec351c4de41b8`  
		Last Modified: Thu, 20 Apr 2023 18:21:09 GMT  
		Size: 114.9 MB (114850123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1caf277928a23fe8d42a293c53757d2249517bdefa1d7278ef0df5b5f7dd8d28`  
		Last Modified: Thu, 20 Apr 2023 18:21:02 GMT  
		Size: 9.1 MB (9106152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2484ae0c639572557e9cde3cd0e9f5d50fdad41be9988a105051130193e06e`  
		Last Modified: Thu, 20 Apr 2023 18:21:01 GMT  
		Size: 858.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a3c7604c9ee2505b6439b95ffbecbccf0afb3b4ff00997edbbf9d101b254bf0`  
		Last Modified: Thu, 20 Apr 2023 18:21:01 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70edb93a4aecd96c2bbde87523c2018634d2d5bc7af75c4a07a3082cdbc52b1f`  
		Last Modified: Thu, 20 Apr 2023 18:21:01 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
