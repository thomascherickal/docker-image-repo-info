## `maven:3-amazoncorretto-8`

```console
$ docker pull maven@sha256:3ba8344c72aeea521879bbb7c69f12487162a3e2539fd6b23dbef52baf173cee
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-8` - linux; amd64

```console
$ docker pull maven@sha256:9de75c77e41c2904a7f43445f2f143705085a3c0cb087ac88a3f36471a23a04e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.0 MB (301047801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43c65d395d9236ef6c23f253583ccd28afe3263c24aafc6f938563fd867512e7`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 05 Jun 2023 19:20:11 GMT
COPY dir:1ad47ba01d0d349e7e7d7ca6f7f5a60739b61c1a0bb68b6f66605d9af77bb0d5 in / 
# Mon, 05 Jun 2023 19:20:12 GMT
CMD ["/bin/bash"]
# Mon, 05 Jun 2023 19:37:25 GMT
ARG version=1.8.0_372.b07-1
# Mon, 05 Jun 2023 19:37:46 GMT
# ARGS: version=1.8.0_372.b07-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 05 Jun 2023 19:37:47 GMT
ENV LANG=C.UTF-8
# Mon, 05 Jun 2023 19:37:47 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Tue, 16 May 2023 11:35:55 GMT
RUN yum install -y tar which gzip # TODO remove # buildkit
# Tue, 16 May 2023 11:35:55 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 16 May 2023 11:35:55 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Tue, 16 May 2023 11:35:55 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Tue, 16 May 2023 11:35:55 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Tue, 16 May 2023 11:35:55 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Tue, 16 May 2023 11:35:55 GMT
ARG MAVEN_VERSION=3.9.2
# Tue, 16 May 2023 11:35:55 GMT
ARG USER_HOME_DIR=/root
# Tue, 16 May 2023 11:35:55 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 16 May 2023 11:35:55 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 16 May 2023 11:35:55 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:a168ccb1c126cd9267eedd2686bc6d0e5415b7fe1009cd832c78ba00655a34d9`  
		Last Modified: Wed, 24 May 2023 21:22:43 GMT  
		Size: 62.5 MB (62493087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573d8989daabd4eea208270e98498a105563ce04e6f09fe7b3e95e6f941d0ecf`  
		Last Modified: Mon, 05 Jun 2023 19:43:26 GMT  
		Size: 75.6 MB (75550664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa79f8c4e3aa3280b734a2d6c7692fe6323e4ac6a6bca8fd6b4c77cb257da69`  
		Last Modified: Mon, 05 Jun 2023 20:23:55 GMT  
		Size: 153.7 MB (153688248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d665bae18091b7f6135cd7d06fbd6e900fdaf7c5023283137d3a36c7323e91b`  
		Last Modified: Mon, 05 Jun 2023 20:23:44 GMT  
		Size: 9.3 MB (9314416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adccae951420994de49b93e066eace265819999b2526c75d3f84bf3de5aeada5`  
		Last Modified: Mon, 05 Jun 2023 20:23:43 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad18a6e8db75bcdee5452c4c3baad935ce37fd7ef7f139e050997bb19096f876`  
		Last Modified: Mon, 05 Jun 2023 20:23:43 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b953f22e1a48e9c5945e8f7c105cac532699842c871514db3e637a80e88095`  
		Last Modified: Mon, 05 Jun 2023 20:23:43 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-8` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:ba2d12fa5cf2082f08750f4ea25ccb24cf22d21a097a4b5f02468c5335010ca6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.6 MB (251641780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08bf96bf2c0147a846948686c93f20fc2dda7752fa0995772f22efb8b52fe39c`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Mon, 05 Jun 2023 19:39:49 GMT
COPY dir:dfd59a801cb05cf6d9b2d75085c49494763e9b18842c146030985cf41b66d3ca in / 
# Mon, 05 Jun 2023 19:39:50 GMT
CMD ["/bin/bash"]
# Mon, 05 Jun 2023 19:55:37 GMT
ARG version=1.8.0_372.b07-1
# Mon, 05 Jun 2023 19:55:53 GMT
# ARGS: version=1.8.0_372.b07-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 05 Jun 2023 19:55:54 GMT
ENV LANG=C.UTF-8
# Mon, 05 Jun 2023 19:55:54 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
# Tue, 16 May 2023 11:35:55 GMT
RUN yum install -y tar which gzip # TODO remove # buildkit
# Tue, 16 May 2023 11:35:55 GMT
ENV MAVEN_HOME=/usr/share/maven
# Tue, 16 May 2023 11:35:55 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Tue, 16 May 2023 11:35:55 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Tue, 16 May 2023 11:35:55 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Tue, 16 May 2023 11:35:55 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Tue, 16 May 2023 11:35:55 GMT
ARG MAVEN_VERSION=3.9.2
# Tue, 16 May 2023 11:35:55 GMT
ARG USER_HOME_DIR=/root
# Tue, 16 May 2023 11:35:55 GMT
ENV MAVEN_CONFIG=/root/.m2
# Tue, 16 May 2023 11:35:55 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Tue, 16 May 2023 11:35:55 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:d916dc829437e3254e7c7e665dd90678298358e7fb563161caa849ca46390827`  
		Last Modified: Wed, 24 May 2023 23:14:13 GMT  
		Size: 64.1 MB (64136791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aadde6114b985017076efddb1be3efe882625cca844a9880e9305bb0651cd5f`  
		Last Modified: Mon, 05 Jun 2023 20:00:33 GMT  
		Size: 59.6 MB (59568680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b453d63fb05cff70b41c6fec7296c62bc9059a9f003749fa0c1d743f42791f6`  
		Last Modified: Mon, 05 Jun 2023 20:28:34 GMT  
		Size: 118.6 MB (118620521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24af13d145efa2eb41065d98fcfba75c62b6d0ea5dfdd12f87ee633449d6821`  
		Last Modified: Mon, 05 Jun 2023 20:28:26 GMT  
		Size: 9.3 MB (9314407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8cfb2f5922a21d3a98dc696f4a4eb10c1cfbd8f7eacc8856e3ca3c7df620c1`  
		Last Modified: Mon, 05 Jun 2023 20:28:25 GMT  
		Size: 856.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c38ed823e5717cc4a882611f3fa4ccdd70630525908d33c1f0659ed58d5a14c`  
		Last Modified: Mon, 05 Jun 2023 20:28:25 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c34b9bfea448bbd923f118c0adb5605f1a3bac611cecd4b07100382b312152`  
		Last Modified: Mon, 05 Jun 2023 20:28:25 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
