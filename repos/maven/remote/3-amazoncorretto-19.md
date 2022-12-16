## `maven:3-amazoncorretto-19`

```console
$ docker pull maven@sha256:23f52a3cfee7cf5bf8373029c439b480a49810e9ee73ec341c95f0b1d263b810
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-19` - linux; amd64

```console
$ docker pull maven@sha256:3c43c057e471c2d75953510ed09a677054b427357fab2042f4d42c99865a55d2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.1 MB (234078132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf98d878eba8684ef1a78fab10354579baf1b89b3f661bf3ee488e2e1d68d61a`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 16 Dec 2022 01:19:49 GMT
ADD file:a69ca7a5499bcd9d6e4317fdbd7256e93be44364bb746f5da10b4268c090bda0 in / 
# Fri, 16 Dec 2022 01:19:50 GMT
CMD ["/bin/bash"]
# Fri, 16 Dec 2022 02:18:05 GMT
ARG version=19.0.1.10-1
# Fri, 16 Dec 2022 02:18:44 GMT
# ARGS: version=19.0.1.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-19-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-19-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 16 Dec 2022 02:18:45 GMT
ENV LANG=C.UTF-8
# Fri, 16 Dec 2022 02:18:45 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-19-amazon-corretto
# Fri, 16 Dec 2022 03:12:28 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Fri, 16 Dec 2022 03:12:29 GMT
ARG MAVEN_VERSION=3.8.6
# Fri, 16 Dec 2022 03:12:29 GMT
ARG USER_HOME_DIR=/root
# Fri, 16 Dec 2022 03:12:29 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Fri, 16 Dec 2022 03:12:29 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Fri, 16 Dec 2022 03:12:30 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 16 Dec 2022 03:12:30 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 16 Dec 2022 03:12:30 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 16 Dec 2022 03:12:30 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 16 Dec 2022 03:12:30 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 16 Dec 2022 03:12:30 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 16 Dec 2022 03:12:30 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:5b4a36b5b78f93a5f470cf722b313bb32cddb0f8e0fa0db348059b5c0881b04f`  
		Last Modified: Thu, 15 Dec 2022 23:08:20 GMT  
		Size: 62.3 MB (62328625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748d50c9408cb82ead9c2f065bb30e9e65b3d4c842cd46e5842d6adc2f1e4a6c`  
		Last Modified: Fri, 16 Dec 2022 02:25:18 GMT  
		Size: 159.4 MB (159380735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b24b88f7ab8f45bc72761ad4e15311d73d47bb60be61ed5ea1922dd495c4da`  
		Last Modified: Fri, 16 Dec 2022 03:15:21 GMT  
		Size: 3.6 MB (3628075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cae6a58367b259d132c0351c14da13ac336883e2d719243c50c28778fac8defa`  
		Last Modified: Fri, 16 Dec 2022 03:15:22 GMT  
		Size: 8.7 MB (8739489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93e139ba5ecdeab2c33e37000d089058b74e6c0b883b79bdd7d90baf21f0e264`  
		Last Modified: Fri, 16 Dec 2022 03:15:21 GMT  
		Size: 851.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd47ab760b78f14826faca3b6525d6c016a095a90723976be04e48d65365e5e`  
		Last Modified: Fri, 16 Dec 2022 03:15:21 GMT  
		Size: 357.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-19` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:6e053123a655c4e85ee42b3c848e2eb42c3be3f1584d6ab3dd079edd8b9e48b7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **234.2 MB (234183858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f7cb3cefefe4d4aa9bd70b709e9e8e1af3f9294e6fb30731002769acfd519b2`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Fri, 16 Dec 2022 00:41:05 GMT
ADD file:26a6bf75c84c408d289e5569f13b1c65206966f875cdfc53ded0670cb85e35bf in / 
# Fri, 16 Dec 2022 00:41:07 GMT
CMD ["/bin/bash"]
# Fri, 16 Dec 2022 01:01:40 GMT
ARG version=19.0.1.10-1
# Fri, 16 Dec 2022 01:01:59 GMT
# ARGS: version=19.0.1.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-19-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-19-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Fri, 16 Dec 2022 01:02:01 GMT
ENV LANG=C.UTF-8
# Fri, 16 Dec 2022 01:02:01 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-19-amazon-corretto
# Fri, 16 Dec 2022 01:22:52 GMT
RUN yum install -y tar which gzip   && rm -rf /var/cache/yum/*   && yum clean all
# Fri, 16 Dec 2022 01:22:52 GMT
ARG MAVEN_VERSION=3.8.6
# Fri, 16 Dec 2022 01:22:52 GMT
ARG USER_HOME_DIR=/root
# Fri, 16 Dec 2022 01:22:52 GMT
ARG SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26
# Fri, 16 Dec 2022 01:22:52 GMT
ARG BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries
# Fri, 16 Dec 2022 01:22:54 GMT
# ARGS: BASE_URL=https://apache.osuosl.org/maven/maven-3/3.8.6/binaries MAVEN_VERSION=3.8.6 SHA=f790857f3b1f90ae8d16281f902c689e4f136ebe584aba45e4b1fa66c80cba826d3e0e52fdd04ed44b4c66f6d3fe3584a057c26dfcac544a60b301e6d0f91c26 USER_HOME_DIR=/root
RUN mkdir -p /usr/share/maven /usr/share/maven/ref   && curl -fsSL -o /tmp/apache-maven.tar.gz ${BASE_URL}/apache-maven-${MAVEN_VERSION}-bin.tar.gz   && echo "${SHA}  /tmp/apache-maven.tar.gz" | sha512sum -c -   && tar -xzf /tmp/apache-maven.tar.gz -C /usr/share/maven --strip-components=1   && rm -f /tmp/apache-maven.tar.gz   && ln -s /usr/share/maven/bin/mvn /usr/bin/mvn
# Fri, 16 Dec 2022 01:22:54 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 16 Dec 2022 01:22:54 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 16 Dec 2022 01:22:54 GMT
COPY file:1b3da5c58894f705e7387946301c0c52edb6271761ea3cd80b86a848847a64cd in /usr/local/bin/mvn-entrypoint.sh 
# Fri, 16 Dec 2022 01:22:54 GMT
COPY file:2bbb488dd73c55d658b91943cfdf9c26975a320ceafc45dda94c95b03e518ad3 in /usr/share/maven/ref/ 
# Fri, 16 Dec 2022 01:22:54 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 16 Dec 2022 01:22:54 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:6cbfee25f0741b3d3f4d2474d904a200cd8404a01aa17813bf3fc3d4ebb551a4`  
		Last Modified: Thu, 15 Dec 2022 23:08:20 GMT  
		Size: 64.0 MB (63964214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a522d703ce658eafb2884db6606c458357c76578aa4a908df5bfdeab0f214a97`  
		Last Modified: Fri, 16 Dec 2022 01:06:12 GMT  
		Size: 157.8 MB (157832709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e542c6b0d8f59679f781e6ee666378e6eb4dd770aa2529d2157146c8917d7cca`  
		Last Modified: Fri, 16 Dec 2022 01:25:10 GMT  
		Size: 3.6 MB (3646238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:865fc40591474c23db75486cfe00f6e8d101b99d7bedb2c8f473727afe408e0a`  
		Last Modified: Fri, 16 Dec 2022 01:25:10 GMT  
		Size: 8.7 MB (8739487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f3419cf13d5c712d6e23821e3e025a3859bde377248d34e6a1e82af530d12b`  
		Last Modified: Fri, 16 Dec 2022 01:25:09 GMT  
		Size: 849.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8694a136df2a06c1c7547058086e4d4ce4ac7303fc45b1ff874a59958f2b37c5`  
		Last Modified: Fri, 16 Dec 2022 01:25:09 GMT  
		Size: 361.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
