## `amazoncorretto:15-alpine`

```console
$ docker pull amazoncorretto@sha256:04b1cf01de8626e8cef4ab413ba47b9f5f31855d524a8d4cf94ecd9adc51e575
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `amazoncorretto:15-alpine` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:c3ffd4ce3ff619e0ed7fdfbf8594a7eab9b89b16fa77638a97efe55c9b391066
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **207.7 MB (207723640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35aa24cc227c0dfd177a26418cd62aa8be9fce11106a20bcf4863fd8c9f758ad`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 13:29:26 GMT
ARG version=15.0.2.7.1
# Thu, 01 Apr 2021 13:29:36 GMT
# ARGS: version=15.0.2.7.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-15=$version-r0
# Thu, 01 Apr 2021 13:29:36 GMT
ENV LANG=C.UTF-8
# Thu, 01 Apr 2021 13:29:36 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Thu, 01 Apr 2021 13:29:37 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b428a93a2ef89e61010a64a2168a6cf214078f1e78d27c293bfa2bb19c866a`  
		Last Modified: Thu, 01 Apr 2021 13:32:22 GMT  
		Size: 204.9 MB (204923928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
