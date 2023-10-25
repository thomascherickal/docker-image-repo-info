## `amazoncorretto:8u392-al2-generic`

```console
$ docker pull amazoncorretto@sha256:0685fa74d1735429cdd2a17ce9d6ab1ce51d814a2bbed7f9efdbc466d25a8dc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:8u392-al2-generic` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:550d370f70da0942583d8bcc2409218fa6e0dfdc614834ea323b0f1baa79d09a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.1 MB (138065400 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cbba2558a98eca3f07e8e54423b26ac8d2eb8a8a2a62b989ca167073d519a0d`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Oct 2023 01:19:53 GMT
COPY dir:fdcfaddab7ba123e1840e939ec5f9c668c54d167449dc297fea5669f294f7222 in / 
# Wed, 25 Oct 2023 01:19:54 GMT
CMD ["/bin/bash"]
# Wed, 25 Oct 2023 01:36:35 GMT
ARG version=1.8.0_392.b08-1
# Wed, 25 Oct 2023 01:36:56 GMT
# ARGS: version=1.8.0_392.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 25 Oct 2023 01:36:56 GMT
ENV LANG=C.UTF-8
# Wed, 25 Oct 2023 01:36:56 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:e6a2a106da1df9b5d4bfa74686415ac760f9d9999604e3784820d596e0983e27`  
		Last Modified: Wed, 25 Oct 2023 01:11:13 GMT  
		Size: 62.5 MB (62492148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:813f830adf0c8b6449c52a3a65b43ec7c3132ca10c7d0e461f0fe0d2757f40a6`  
		Last Modified: Wed, 25 Oct 2023 01:52:21 GMT  
		Size: 75.6 MB (75573252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:8u392-al2-generic` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:d5dda4c5d788b1ffe6b84abc4379929fc66cffccdff09fe66b6d478d1bf5da8c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.8 MB (123830407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2977dc01c65c49da3d3cbdc090920d44256b163a639117dfc30809594e0f8675`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 25 Oct 2023 00:39:44 GMT
COPY dir:8cce6e6a6abbbd299b12dd9d8f9974415975c25f4170a182c4d6addd8ba9d101 in / 
# Wed, 25 Oct 2023 00:39:45 GMT
CMD ["/bin/bash"]
# Wed, 25 Oct 2023 01:17:36 GMT
ARG version=1.8.0_392.b08-1
# Wed, 25 Oct 2023 01:17:54 GMT
# ARGS: version=1.8.0_392.b08-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-1.8.0-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-1.8.0-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 25 Oct 2023 01:17:55 GMT
ENV LANG=C.UTF-8
# Wed, 25 Oct 2023 01:17:55 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-1.8.0-amazon-corretto
```

-	Layers:
	-	`sha256:bceed9d4335ecd25da3cee660b39ab03c762b3e6bc197470f6eeeaad4c7f3db4`  
		Last Modified: Wed, 25 Oct 2023 00:40:19 GMT  
		Size: 64.2 MB (64228438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf0613259b21f18eae16fda9a47282ff07bdb48811375355261d047145edb0d`  
		Last Modified: Wed, 25 Oct 2023 01:27:45 GMT  
		Size: 59.6 MB (59601969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
