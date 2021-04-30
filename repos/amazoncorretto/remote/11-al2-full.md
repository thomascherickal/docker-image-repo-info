## `amazoncorretto:11-al2-full`

```console
$ docker pull amazoncorretto@sha256:b614d9ffdf2a29606fbf6a9aa7df29cae62a9f1ce798f5f92ef7ddb18f5691cd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:8445724e9167070365db67b8ecc646d5c536689c1d88422be73ed66112b1e277
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.6 MB (208615695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:123fb0591749d235c85a15645875e5610c476794b856d7be33c08f39ae493c89`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 29 Apr 2021 22:25:37 GMT
ADD file:47fcf0318dccec16b61a0d21a0f16c45b77dea5abf50ba6604f1ffadcb299d10 in / 
# Thu, 29 Apr 2021 22:25:38 GMT
CMD ["/bin/bash"]
# Thu, 29 Apr 2021 22:44:48 GMT
ARG version=11.0.11.9-1
# Thu, 29 Apr 2021 22:45:13 GMT
# ARGS: version=11.0.11.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 29 Apr 2021 22:45:13 GMT
ENV LANG=C.UTF-8
# Thu, 29 Apr 2021 22:45:14 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:3c2c91c7c4311eca863331479504040ee4f45fda9a610947b82886e7bbd5b737`  
		Last Modified: Thu, 29 Apr 2021 22:27:18 GMT  
		Size: 61.9 MB (61947132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17eb3d153b3376801c1da7fc410637e77e5b7e2891bf6e58d32dc6a02ab1473a`  
		Last Modified: Thu, 29 Apr 2021 22:47:15 GMT  
		Size: 146.7 MB (146668563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:13bd2f785e81f532fbe52bc69976e45f436171f6c9240819117013ac51432461
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **208.4 MB (208406492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bd2aa6f5ce02099d19071644500cc0376d7698e85ccd840b34039755bdc4013`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 29 Apr 2021 22:40:32 GMT
ADD file:03605b69274d89b78234df03d53dacc9cac408d68b82b1fb5d63b84c01b69300 in / 
# Thu, 29 Apr 2021 22:40:37 GMT
CMD ["/bin/bash"]
# Thu, 29 Apr 2021 22:59:09 GMT
ARG version=11.0.11.9-1
# Thu, 29 Apr 2021 22:59:48 GMT
# ARGS: version=11.0.11.9-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Thu, 29 Apr 2021 22:59:50 GMT
ENV LANG=C.UTF-8
# Thu, 29 Apr 2021 22:59:50 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:316be4ce82c0add9f71a6ce1face38b99f456abd45232cf7ad96ccac098ef5fe`  
		Last Modified: Thu, 29 Apr 2021 22:41:52 GMT  
		Size: 63.7 MB (63660068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f95858667f8940b79869dc419ce2be62c27d5e0291f6dfd0e8829db451947c2d`  
		Last Modified: Thu, 29 Apr 2021 23:01:52 GMT  
		Size: 144.7 MB (144746424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
