## `maven:3-amazoncorretto-20-debian-bookworm`

```console
$ docker pull maven@sha256:b34231af2d7fae0fa9b5f2e438f1514c678cfda4868343808207f5b9371480d9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `maven:3-amazoncorretto-20-debian-bookworm` - linux; amd64

```console
$ docker pull maven@sha256:48eafcd57f45666a7531e2e4f111a3b80deef0e56b501e07071e26d6d6dc7d9b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.4 MB (246445603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5aa6f560402bfb9fadd3e31446ac1479b8d1801ca5f4ddbfd29d8e220e3e57f`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 20 Sep 2023 04:55:40 GMT
ADD file:a1398394375faab8dd9e1e8d584eea96c750fb57ae4ffd2b14624f1cf263561b in / 
# Wed, 20 Sep 2023 04:55:41 GMT
CMD ["bash"]
# Fri, 18 Aug 2023 15:26:34 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-20-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 18 Aug 2023 15:26:34 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
ARG MAVEN_VERSION=3.9.4
# Fri, 18 Aug 2023 15:26:34 GMT
ARG USER_HOME_DIR=/root
# Fri, 18 Aug 2023 15:26:34 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 18 Aug 2023 15:26:34 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 18 Aug 2023 15:26:34 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:a803e7c4b030119420574a882a52b6431e160fceb7620f61b525d49bc2d58886`  
		Last Modified: Wed, 20 Sep 2023 05:00:22 GMT  
		Size: 29.1 MB (29124705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ec7cc223b20272e6f01e420851fd22da6949379cced1d1446f0457b7e60190a`  
		Last Modified: Wed, 20 Sep 2023 09:13:18 GMT  
		Size: 207.9 MB (207913107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fff1a642e6a0c1e49bfff9d0c2069f691fe132b3e92956ae3cf12b5cc1477ecb`  
		Last Modified: Wed, 20 Sep 2023 09:13:04 GMT  
		Size: 9.4 MB (9406412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c55336ce7a6a9926be085215a0698d19ce4fcf8cfbf24750e76b214c5ba5d4e`  
		Last Modified: Wed, 20 Sep 2023 09:13:03 GMT  
		Size: 854.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775f422a560aec71a365d37188b907bad90645e61650828c9c12cae6230ff091`  
		Last Modified: Wed, 20 Sep 2023 09:13:03 GMT  
		Size: 358.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f4b1abc6ec653e991b6b3fddb4aeaa6f1232f84b95a2db55bd76e68cca2bc68`  
		Last Modified: Wed, 20 Sep 2023 09:13:03 GMT  
		Size: 167.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `maven:3-amazoncorretto-20-debian-bookworm` - linux; arm64 variant v8

```console
$ docker pull maven@sha256:d7d8bdd59602682213fd41b8618886266ea54fd68cd07e6dba3d2f1bba667666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **244.3 MB (244316440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:902f0e91108636e388de6d761db8a26a83dc1c7f00b4c847e4391a451aed300d`
-	Entrypoint: `["\/usr\/local\/bin\/mvn-entrypoint.sh"]`
-	Default Command: `["mvn"]`

```dockerfile
# Wed, 20 Sep 2023 02:44:13 GMT
ADD file:ec1a6e0aedd76c8fdc8544775f8b553f58950e9435f5cfe919f39374e222cfbb in / 
# Wed, 20 Sep 2023 02:44:14 GMT
CMD ["bash"]
# Fri, 18 Aug 2023 15:26:34 GMT
RUN apt-get update   && apt-get install -y curl gnupg   && export GNUPGHOME="$(mktemp -d)"   && curl -fL https://apt.corretto.aws/corretto.key | gpg --batch --import   && gpg --batch --export '6DC3636DAE534049C8B94623A122542AB04F24E3' > /usr/share/keyrings/corretto.gpg   && rm -r "$GNUPGHOME"   && unset GNUPGHOME   && echo "deb [signed-by=/usr/share/keyrings/corretto.gpg] https://apt.corretto.aws stable main" > /etc/apt/sources.list.d/corretto.list   && apt-get update   && apt-get remove --purge --autoremove -y curl gnupg   && apt-get install -y java-20-amazon-corretto-jdk   && rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
ENV MAVEN_HOME=/usr/share/maven
# Fri, 18 Aug 2023 15:26:34 GMT
COPY /usr/share/maven /usr/share/maven # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
COPY /usr/local/bin/mvn-entrypoint.sh /usr/local/bin/mvn-entrypoint.sh # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
COPY /usr/share/maven/ref/settings-docker.xml /usr/share/maven/ref/settings-docker.xml # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
RUN ln -s ${MAVEN_HOME}/bin/mvn /usr/bin/mvn # buildkit
# Fri, 18 Aug 2023 15:26:34 GMT
ARG MAVEN_VERSION=3.9.4
# Fri, 18 Aug 2023 15:26:34 GMT
ARG USER_HOME_DIR=/root
# Fri, 18 Aug 2023 15:26:34 GMT
ENV MAVEN_CONFIG=/root/.m2
# Fri, 18 Aug 2023 15:26:34 GMT
ENTRYPOINT ["/usr/local/bin/mvn-entrypoint.sh"]
# Fri, 18 Aug 2023 15:26:34 GMT
CMD ["mvn"]
```

-	Layers:
	-	`sha256:e886f0f47ef56fcadb6ecaf2116056bbdb273e0afe07ed034498b198d386c04e`  
		Last Modified: Wed, 20 Sep 2023 02:47:36 GMT  
		Size: 29.2 MB (29157221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4823b1b180ec801eb8d19c294ae1ec4ad7dc3377af22786f5af071ba7a988b3d`  
		Last Modified: Wed, 20 Sep 2023 12:29:49 GMT  
		Size: 205.8 MB (205751400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a560a994c177e51cb0021511040185de4807266baa59aa58ae9ee0cd9c32e9`  
		Last Modified: Wed, 20 Sep 2023 12:29:37 GMT  
		Size: 9.4 MB (9406439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6d6c7e52b08fba9d1b323385ae3462521910fa20e51da7198fd82510f90bc6`  
		Last Modified: Wed, 20 Sep 2023 12:29:36 GMT  
		Size: 855.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1991991c5bb2a6ef6439a8eddc51dbacef32bac0777fc39b7296bd5958ed416d`  
		Last Modified: Wed, 20 Sep 2023 12:29:36 GMT  
		Size: 360.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51443cf4270d38817a24df75c5da088ff817e3590bf95e00be5b602217856470`  
		Last Modified: Wed, 20 Sep 2023 12:29:36 GMT  
		Size: 165.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
