## `amazoncorretto:15-al2-jdk`

```console
$ docker pull amazoncorretto@sha256:df04cb1319a2c5d2fd0ef20b3a2c3bf7bdb66898f12843f667948f2435f23b60
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:15-al2-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:5ca527dc41ba6947e6ca81a944a3e0b3065ba530a40c04df37d6b39298881292
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.3 MB (217321840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:490bde902fa3a33e5a5e0aab40c6333eaa3ea13574e97827cdcd6003c2557568`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:19:45 GMT
ADD file:92220f428664788288d5cda805c94b48f6a5e957d4c7724085f3278d0a864f6d in / 
# Fri, 31 Jul 2020 22:19:46 GMT
CMD ["/bin/bash"]
# Mon, 12 Oct 2020 23:19:29 GMT
ARG version=15.0.0.36-1
# Mon, 12 Oct 2020 23:19:55 GMT
# ARGS: version=15.0.0.36-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 12 Oct 2020 23:19:55 GMT
ENV LANG=C.UTF-8
# Mon, 12 Oct 2020 23:19:56 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:37373184fe69e0fc20370c26317bf4c5b9b843c60b375563d4ee1c7766a89782`  
		Last Modified: Fri, 31 Jul 2020 22:20:37 GMT  
		Size: 61.7 MB (61716540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2854c7d8fc6af180bfd359fa713f1ca4977a1aa067ede0c5fb3750c9e8dd7f6b`  
		Last Modified: Mon, 12 Oct 2020 23:21:10 GMT  
		Size: 155.6 MB (155605300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:15-al2-jdk` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:e4d52794e15ee02085555784e477eb1de6061dba4bcd9fa44173156cd9768645
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.8 MB (218839873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694d0842ba570a080b6465355d894bb98325324ba18d9005061b06c63b47345c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 31 Jul 2020 22:43:15 GMT
ADD file:d4c394189445aecbba87f3effbedda61d337d18393fa4b1af22ce498be6f6af0 in / 
# Fri, 31 Jul 2020 22:43:20 GMT
CMD ["/bin/bash"]
# Mon, 12 Oct 2020 23:52:59 GMT
ARG version=15.0.0.36-1
# Mon, 12 Oct 2020 23:53:44 GMT
# ARGS: version=15.0.0.36-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && yum install -y java-15-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-15-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Mon, 12 Oct 2020 23:53:46 GMT
ENV LANG=C.UTF-8
# Mon, 12 Oct 2020 23:53:46 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-15-amazon-corretto
```

-	Layers:
	-	`sha256:c9ca78f6e1f39219972cf4f8dac027e6f91e01d68c7aefd9c55b86c47f558827`  
		Last Modified: Fri, 31 Jul 2020 22:44:30 GMT  
		Size: 63.4 MB (63354136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9cec919617a88eeabffbf23ba397a8d0242ca3c914df2b6bd7d7b0e73b12e6`  
		Last Modified: Mon, 12 Oct 2020 23:54:34 GMT  
		Size: 155.5 MB (155485737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
