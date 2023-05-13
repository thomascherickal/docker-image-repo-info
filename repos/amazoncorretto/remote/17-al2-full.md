## `amazoncorretto:17-al2-full`

```console
$ docker pull amazoncorretto@sha256:df859d03b99446cd10ecddc7f9a9096d1ad5fc87a050b7e91f4711310dcbf8bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:17-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:556cc24637289c56e84d811fe600157747d380f760612c43d9efd33da11a5ce5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.5 MB (214468752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:212361430699e9f058bcd4573bae99dc8d54a0dc8205d90d9e2471a9c7765380`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Sat, 13 May 2023 00:19:34 GMT
COPY dir:7a824a76678fb4ef17879dcecd9fac65df3d1efbef31a3b874da9f49f49b6814 in / 
# Sat, 13 May 2023 00:19:34 GMT
CMD ["/bin/bash"]
# Sat, 13 May 2023 01:34:17 GMT
ARG version=17.0.7.7-1
# Sat, 13 May 2023 01:34:42 GMT
# ARGS: version=17.0.7.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Sat, 13 May 2023 01:34:43 GMT
ENV LANG=C.UTF-8
# Sat, 13 May 2023 01:34:43 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:bf72c394abb748707ec4590d5017f36ad47098c9b92adc1b04c3ea3ba0b395f6`  
		Last Modified: Fri, 12 May 2023 00:07:44 GMT  
		Size: 62.5 MB (62494714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4edf64cf85c039184023bdfaa7e82e8a607c7f0a55286cce0c938431af0d83d3`  
		Last Modified: Sat, 13 May 2023 01:37:36 GMT  
		Size: 152.0 MB (151974038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:17-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:df0bee176db3c4f85cbfde87c103d5e1df1b35ea13ede735e9d769cda88ea138
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.6 MB (214622930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab629d077f87bbd3efd3860bde0b4a3f1bdd2952a8a3974d9745f7a0afc41dd8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 04 May 2023 20:02:54 GMT
COPY dir:dcba415a4a8d9f29c0f5914e2b9ce92b35bd4109c9cd4a8feba13044e94360bf in / 
# Thu, 04 May 2023 20:02:55 GMT
CMD ["/bin/bash"]
# Thu, 04 May 2023 21:17:43 GMT
ARG version=17.0.7.7-1
# Thu, 04 May 2023 21:18:02 GMT
# ARGS: version=17.0.7.7-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-17-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-17-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 04 May 2023 21:18:04 GMT
ENV LANG=C.UTF-8
# Thu, 04 May 2023 21:18:04 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-17-amazon-corretto
```

-	Layers:
	-	`sha256:7691241ca28307f278612dad94d3164926fb17e58a2302a47349e0d6e001249e`  
		Last Modified: Tue, 25 Apr 2023 06:49:36 GMT  
		Size: 64.1 MB (64130990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b5eea751fa7fbb48aeb35861b4a78f5be366c3bf2bcc1e2c47aa89b579ded92`  
		Last Modified: Thu, 04 May 2023 21:22:36 GMT  
		Size: 150.5 MB (150491940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
