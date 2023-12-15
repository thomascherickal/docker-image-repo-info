## `maven:amazoncorretto`

```console
$ docker pull maven@sha256:1206d8e9cd9de373278e3afdd172ba8b85f95760c5413e56d76d496a6e94626a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:amazoncorretto` - linux; amd64

```console
$ docker pull maven@sha256:5af6beb7386176992201798907e62df7160a893177a50cb61b4470c098dac698
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.2 MB (365185686 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b91aeecff9130596018b11ffb9a1fbde6e1b566a16cfaa708ba87ebc0beec4ba`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 15 Dec 2023 20:22:49 GMT
COPY dir:fd6bc3e61b31127123e1a8c57613d9baa7f5605d29d858f885c6a105709aa8fd in / 
# Fri, 15 Dec 2023 20:22:50 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 20:42:41 GMT
ARG version=11.0.21.9-1
# Fri, 15 Dec 2023 20:43:04 GMT
# ARGS: version=11.0.21.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 15 Dec 2023 20:43:04 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 20:43:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Mon, 11 Dec 2023 11:12:11 GMT
RUN yum install -y tar which gzip # TODO remove # buildkit
# Mon, 11 Dec 2023 11:12:11 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 11 Dec 2023 11:12:11 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Mon, 11 Dec 2023 11:12:11 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Mon, 11 Dec 2023 11:12:11 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Mon, 11 Dec 2023 11:12:11 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Mon, 11 Dec 2023 11:12:11 GMT
ARG MAVEN_VERSION=3.9.6
# Mon, 11 Dec 2023 11:12:11 GMT
ARG USER_HOME_DIR=/root
# Mon, 11 Dec 2023 11:12:11 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 11 Dec 2023 11:12:11 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 11 Dec 2023 11:12:11 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:497f6fc6e5d7835e37c10dd6462da0d293dc146b7ead757dc61e580b47fd2578`  
		Last Modified: Tue, 12 Dec 2023 02:10:17 GMT  
		Size: 62.6 MB (62645650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3e13fc6d99aa0e7f4421920aa7183cbfdcf085462a8bc98d4843d02a3bdeb0f`  
		Last Modified: Fri, 15 Dec 2023 20:54:45 GMT  
		Size: 147.9 MB (147943952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ace39167f3a55455c6257dcdc2ed9301516f3201e8961202417d90b4c6365a4`  
		Last Modified: Fri, 15 Dec 2023 21:52:36 GMT  
		Size: 145.1 MB (145114751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e027d67d2cbafcc7ccfcc77b800a3f560390df92aa3cef42f2cd85c86a4c850e`  
		Last Modified: Fri, 15 Dec 2023 21:52:24 GMT  
		Size: 9.5 MB (9479948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c88154f1ef18d7f3ddcc08fd8ee4f8cf203cbdfff00dedbae2395183c71ec8c`  
		Last Modified: Fri, 15 Dec 2023 21:52:23 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b21648d61f2449223fbee3a568bcf829c9b11204a7cc6c032e972d9531daceb`  
		Last Modified: Fri, 15 Dec 2023 21:52:23 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cba6a0b8877d9c84ab2b334e4ecc17ef59997516ebcd7f7c61567ae3ee6db4`  
		Last Modified: Fri, 15 Dec 2023 21:52:23 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:amazoncorretto` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:679c416d7eac1fc7d0a151150b7aef8e1d0e35540b66de57397c655c4b38659e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.9 MB (334925631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f169e75cacaa4bd5b34423660a4b1c02b5c66deab235e22f4a27a92d8605b98`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 15 Dec 2023 20:44:39 GMT
COPY dir:10ec8ba603fc9dc4661d37af0490e95262fb40302640f3ade11c9c85291feebb in / 
# Fri, 15 Dec 2023 20:44:40 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 21:10:27 GMT
ARG version=11.0.21.9-1
# Fri, 15 Dec 2023 21:10:45 GMT
# ARGS: version=11.0.21.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 15 Dec 2023 21:10:47 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 21:10:47 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
# Mon, 11 Dec 2023 11:12:11 GMT
RUN yum install -y tar which gzip # TODO remove # buildkit
# Mon, 11 Dec 2023 11:12:11 GMT
ENV MAVEN_HOME=/usr/share/maven
# Mon, 11 Dec 2023 11:12:11 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Mon, 11 Dec 2023 11:12:11 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Mon, 11 Dec 2023 11:12:11 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Mon, 11 Dec 2023 11:12:11 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Mon, 11 Dec 2023 11:12:11 GMT
ARG MAVEN_VERSION=3.9.6
# Mon, 11 Dec 2023 11:12:11 GMT
ARG USER_HOME_DIR=/root
# Mon, 11 Dec 2023 11:12:11 GMT
ENV MAVEN_CONFIG=/root/.m2
# Mon, 11 Dec 2023 11:12:11 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Mon, 11 Dec 2023 11:12:11 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:770064597beb3d761f91ecebb678371619bec21864a4248afd29b220625976f2`  
		Last Modified: Tue, 12 Dec 2023 08:31:57 GMT  
		Size: 64.4 MB (64444817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5bf360129e802cfe2ba2c878453267103f20b71c447b441d51732d46ecaf219`  
		Last Modified: Fri, 15 Dec 2023 21:19:53 GMT  
		Size: 145.0 MB (145011974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d230f55d01da5e458b120c5fb2daef3010644e04ea87d7b308bf77908cec25`  
		Last Modified: Fri, 15 Dec 2023 21:43:56 GMT  
		Size: 116.0 MB (115987515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8390ec4d53bea3985a920b7ee9cf8f20aedcfb98f113cb671ec93de80a98e5f5`  
		Last Modified: Fri, 15 Dec 2023 21:43:48 GMT  
		Size: 9.5 MB (9479943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485304be00c0ab499c5a74bae1b62a1e3df179444bee98c412df8ddb1e7ca7fe`  
		Last Modified: Fri, 15 Dec 2023 21:43:47 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46a097c16b66619850693e13619e8f38bd00d24ea11eaa01c4b9791d43cd7a2`  
		Last Modified: Fri, 15 Dec 2023 21:43:47 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1426abfcd58d1ed0044e3f1293a91a5f7c0ecb6a47e0c72fafaeba2a26ba5ea7`  
		Last Modified: Fri, 15 Dec 2023 21:43:47 GMT  
		Size: 166.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
