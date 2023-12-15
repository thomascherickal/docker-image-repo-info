## `maven:3-amazoncorretto-21`

```console
$ docker pull maven@sha256:7f74504ae14c07df524998d895d7696c8da2ac0126c06bc76bbe0680f4bc82b4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-21` - linux; amd64

```console
$ docker pull maven@sha256:f08c059f4c3a6a5d4984993577c6603f341c46629fa48a50f3ea91c0d6561b12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **382.7 MB (382722439 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3e350a4e30f9de044bc56a19c934fd4e940ecd8e0947d9d8e876d98009aecf6`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 15 Dec 2023 20:22:49 GMT
COPY dir:fd6bc3e61b31127123e1a8c57613d9baa7f5605d29d858f885c6a105709aa8fd in / 
# Fri, 15 Dec 2023 20:22:50 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 20:49:42 GMT
ARG version=21.0.1.12-1
# Fri, 15 Dec 2023 20:50:06 GMT
# ARGS: version=21.0.1.12-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-21-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-21-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 15 Dec 2023 20:50:07 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 20:50:07 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
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
	-	`sha256:3d6a10c4f7ceee0807d59ee5ccde088895b637676672dc6a17ecd82c02419c79`  
		Last Modified: Fri, 15 Dec 2023 20:59:45 GMT  
		Size: 165.5 MB (165482822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a3df2373e56ca0e25a1108845db444363bcb59923380338166161f4aeca9c1`  
		Last Modified: Fri, 15 Dec 2023 21:54:02 GMT  
		Size: 145.1 MB (145112636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:222e5238b47907d70630fc8825de252a5228388662c545259d6f4d67f6f9046b`  
		Last Modified: Fri, 15 Dec 2023 21:53:50 GMT  
		Size: 9.5 MB (9479946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24c958c19cf946c658c5b7d2edb4e4c496a44af4be2e358b4bb3653c00adacf`  
		Last Modified: Fri, 15 Dec 2023 21:53:49 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285e97a2f444b4f8caabaf5f1e961774ce96881f68e54bd468aaca064d9994db`  
		Last Modified: Fri, 15 Dec 2023 21:53:49 GMT  
		Size: 362.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0779e35ca516bf5d9ab6e3612dd02958bc84dea8ac689f2c47feedd7942681b3`  
		Last Modified: Fri, 15 Dec 2023 21:53:50 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-21` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:8e83c7cc45ba036437bc8ae11b2b99f322b8668d224c5f80d1ecd53afa81fe9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.4 MB (353363373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03668f83c1cad560aad5a960365127186b63aa0560f43119ddce16d659cbd799`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 15 Dec 2023 20:44:39 GMT
COPY dir:10ec8ba603fc9dc4661d37af0490e95262fb40302640f3ade11c9c85291feebb in / 
# Fri, 15 Dec 2023 20:44:40 GMT
CMD ["/bin/bash"]
# Fri, 15 Dec 2023 21:15:57 GMT
ARG version=21.0.1.12-1
# Fri, 15 Dec 2023 21:16:17 GMT
# ARGS: version=21.0.1.12-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-21-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-21-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 15 Dec 2023 21:16:19 GMT
ENV LANG=C.UTF-8
# Fri, 15 Dec 2023 21:16:19 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-21-amazon-corretto
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
	-	`sha256:b84a22ddf532a229c35b3bc1a6de42b3b347a9eca7be835dac1ca71fcb8cf22d`  
		Last Modified: Fri, 15 Dec 2023 21:24:10 GMT  
		Size: 163.5 MB (163453105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0693e815d25871f4b04db45531a62325aab85bee9e15c3f1c9489b49c928454`  
		Last Modified: Fri, 15 Dec 2023 21:46:50 GMT  
		Size: 116.0 MB (115984138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc0f0e6209eb00d5d55bd7071d96ce48d3a9200d941ba785f802826cf519670`  
		Last Modified: Fri, 15 Dec 2023 21:46:42 GMT  
		Size: 9.5 MB (9479932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d1a05fbc5cf48d66da789558a0e1c401f46a77e55ebcee4a286deca18b39a0`  
		Last Modified: Fri, 15 Dec 2023 21:46:41 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fbe53e5164344f4640bffa771793e9db22bd5abd49d534cc3c696819fd0cd20`  
		Last Modified: Fri, 15 Dec 2023 21:46:41 GMT  
		Size: 359.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e072d75db0c26da88ea99bd6f38bef0e9159e124c6834bc665d439582924582c`  
		Last Modified: Fri, 15 Dec 2023 21:46:41 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
