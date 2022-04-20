## `amazoncorretto:18-al2-full`

```console
$ docker pull amazoncorretto@sha256:281bc9fad6547994619257f867f29ac664b643d06c46d392301a65c8582f0736
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `amazoncorretto:18-al2-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:d12f38b8ace3800cbe8f231b2f51c6db0ed657867a5f26731e5373b58fc5dcb1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.9 MB (214931444 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5e1721265e60af59d6093905d421425979e10a355ed7fef6aca1f8375d91a73`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 13 Apr 2022 21:26:09 GMT
ADD file:7fa33984010a56e1ee5aa401253e0d989c79d49005db9c39461482307d209f33 in / 
# Wed, 13 Apr 2022 21:26:10 GMT
CMD ["/bin/bash"]
# Tue, 19 Apr 2022 22:26:06 GMT
ARG version=18.0.1.10-1
# Tue, 19 Apr 2022 22:26:38 GMT
# ARGS: version=18.0.1.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-18-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-18-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 19 Apr 2022 22:26:38 GMT
ENV LANG=C.UTF-8
# Tue, 19 Apr 2022 22:26:39 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-18-amazon-corretto
```

-	Layers:
	-	`sha256:b4b6ff8728329c46c11473e599b18813271c5059023956140f08ecaf87f7859a`  
		Last Modified: Wed, 13 Apr 2022 02:49:33 GMT  
		Size: 62.2 MB (62237641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f68f69811631935041c854290d585749e03756fe62e3571603585fd8871176f`  
		Last Modified: Tue, 19 Apr 2022 22:37:32 GMT  
		Size: 152.7 MB (152693803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `amazoncorretto:18-al2-full` - linux; arm64 variant v8

```console
$ docker pull amazoncorretto@sha256:f5cbf4e603232b331c68cb5cfaac2acb264c0085fc5bacaa9ad437b035ca2e4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **215.2 MB (215231473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc7cf86f459ffbce965550fb247f30a2a834acb4945009595b7da62e871a3198`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 13 Apr 2022 21:39:23 GMT
ADD file:b2ebb2642f1562a48fcb84ac23c60719e85ce47ae98e58a9c3b80e90779c96bc in / 
# Wed, 13 Apr 2022 21:39:24 GMT
CMD ["/bin/bash"]
# Tue, 19 Apr 2022 21:40:37 GMT
ARG version=18.0.1.10-1
# Tue, 19 Apr 2022 21:40:54 GMT
# ARGS: version=18.0.1.10-1
RUN set -eux     && export GNUPGHOME="$(mktemp -d)"     && curl -fL -o corretto.key https://yum.corretto.aws/corretto.key     && gpg --batch --import corretto.key     && gpg --batch --export --armor '6DC3636DAE534049C8B94623A122542AB04F24E3' > corretto.key     && rpm --import corretto.key     && rm -r "$GNUPGHOME" corretto.key     && curl -fL -o /etc/yum.repos.d/corretto.repo https://yum.corretto.aws/corretto.repo     && grep -q '^gpgcheck=1' /etc/yum.repos.d/corretto.repo     && echo "priority=9" >> /etc/yum.repos.d/corretto.repo     && yum install -y java-18-amazon-corretto-devel-$version     && (find /usr/lib/jvm/java-18-amazon-corretto -name src.zip -delete || true)     && yum install -y fontconfig     && yum clean all
# Tue, 19 Apr 2022 21:40:55 GMT
ENV LANG=C.UTF-8
# Tue, 19 Apr 2022 21:40:55 GMT
ENV JAVA_HOME=/usr/lib/jvm/java-18-amazon-corretto
```

-	Layers:
	-	`sha256:7072f8fc5d0e256808f60aaf5dc2a7b918f5094683b66be0a216b4e8a859ee10`  
		Last Modified: Wed, 13 Apr 2022 02:49:29 GMT  
		Size: 63.9 MB (63870281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b34ff630bcf287771daa105900e97433ca90125b6f7360ed9b0738586b19af`  
		Last Modified: Tue, 19 Apr 2022 21:43:44 GMT  
		Size: 151.4 MB (151361192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
