## `amazoncorretto:11-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:23b3da2fac66d1802226298da373a6c5d1560a621309c7dd2c72a7e26686190f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:11-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:595d3791e579d4a17c238b6c657ec1d585f15acad53670fd7cda83193cab2e30
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.7 MB (206745743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcce9e8293ec543246f18c626211aeb0370304e1e0d9afa78ebfd102fbef98ec`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Apr 2020 18:22:56 GMT
ADD file:c64a7d77d1e9f4364c8d2009059cb8668697d61f54f457215b6be6f0c9cded5b in / 
# Tue, 21 Apr 2020 18:22:56 GMT
CMD ["/bin/bash"]
# Tue, 21 Apr 2020 18:51:29 GMT
ARG version=11.0.7.10-1
# Wed, 29 Apr 2020 23:20:27 GMT
# ARGS: version=11.0.7.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 29 Apr 2020 23:20:27 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:a3f8e652bdc470bbea38766fe41f8f12b9e4d44e9ce4037eb502839754b06b9c`  
		Last Modified: Tue, 21 Apr 2020 18:23:48 GMT  
		Size: 61.6 MB (61619066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d195fe3929b2a2dd78d22148b5ee06df7ffc52f14a78429cf5f833e0e26c9fe5`  
		Last Modified: Wed, 29 Apr 2020 23:21:08 GMT  
		Size: 145.1 MB (145126677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:11-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:9e555d383bfb92906790f4e8fefc46308dc2334a74100c5cba1c4e807f9957fb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.0 MB (207042957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb41125d330979c841d226f6a14805bef245b10d9ab4ae62a3c7e0e3bb31494e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 21 Apr 2020 18:58:16 GMT
ADD file:85fc0908f460f80c41755d2b5ab9ff6a025bb2726628ccc4edceb21d2e3f8edf in / 
# Tue, 21 Apr 2020 18:58:18 GMT
CMD ["/bin/bash"]
# Tue, 21 Apr 2020 19:26:46 GMT
ARG version=11.0.7.10-1
# Wed, 29 Apr 2020 23:40:57 GMT
# ARGS: version=11.0.7.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-11-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-11-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Wed, 29 Apr 2020 23:40:59 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-11-amazon-corretto
```

-	Layers:
	-	`sha256:0a37a5cd26f245ce54aff575389ef7765520d37d3ea7c437144c936c6adffc8a`  
		Last Modified: Tue, 21 Apr 2020 18:59:54 GMT  
		Size: 63.1 MB (63079760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc719ce9c572714bce34bed2d488330731b35adac7227db1447baef738078401`  
		Last Modified: Wed, 29 Apr 2020 23:42:00 GMT  
		Size: 144.0 MB (143963197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
