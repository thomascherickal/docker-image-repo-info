## `amazoncorretto:8-alpine3.15-jre`

```console
$ docker pull amazoncorretto@sha256:1504ea70ea5b602c91f5422dbfc8908eb3b678e69338a4f29ce882fef4a070ab
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:8-alpine3.15-jre` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:08f90eef7c6d050b840b2e622f3f8ad7cdb8f222ae93d1f0ffb5b6c7e963d917
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43222401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7deb900d0f0f8cc848bb7a8647bc25ed4961dc94fd262958f42d061f6e00b60c`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 19 Apr 2022 22:23:33 GMT
ARG version=8.332.08.1
# Tue, 19 Apr 2022 22:23:43 GMT
# ARGS: version=8.332.08.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-8-jre=$version-r0 &&     ln -s -f ../lib/jvm/default-jvm/jre/bin/java /usr/bin/java &&     ln -s -f ../lib/jvm/default-jvm/jre/bin/jjs /usr/bin/jjs &&     ln -s -f ../lib/jvm/default-jvm/jre/bin/keytool /usr/bin/keytool &&     ln -s -f ../lib/jvm/default-jvm/jre/bin/pack200 /usr/bin/pack200 &&     ln -s -f ../lib/jvm/default-jvm/jre/bin/rmid /usr/bin/rmid &&     ln -s -f ../lib/jvm/default-jvm/jre/bin/rmiregistry /usr/bin/rmiregistry &&     ln -s -f ../lib/jvm/default-jvm/jre/bin/unpack200 /usr/bin/unpack200
# Tue, 19 Apr 2022 22:23:43 GMT
ENV LANG=C.UTF-8
# Tue, 19 Apr 2022 22:23:43 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm/jre
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ef211f1e56ca8fc3a7a0b9aaff99651225a85daa938e07928e98a87538ad4b`  
		Last Modified: Tue, 19 Apr 2022 22:31:59 GMT  
		Size: 40.4 MB (40407842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
