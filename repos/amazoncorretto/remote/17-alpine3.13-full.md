## `amazoncorretto:17-alpine3.13-full`

```console
$ docker pull amazoncorretto@sha256:1fc9cd3d7539f87376ba9077be1acefdf3786dff9a6c971c8049a71b58a24251
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:17-alpine3.13-full` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:8f8fc42792cf4347df2a0dc7c00dabf862f5cf46bc204178b5d8dddc0b60c165
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.6 MB (194571782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c54caa024ead1bbaf8558cd69c66264deb1baa6174a00184b88df1e64bf541c7`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Mon, 25 Oct 2021 18:24:42 GMT
ARG version=17.0.1.12.1
# Mon, 25 Oct 2021 18:24:48 GMT
# ARGS: version=17.0.1.12.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-17=$version-r0
# Mon, 25 Oct 2021 18:24:48 GMT
ENV LANG=C.UTF-8
# Mon, 25 Oct 2021 18:24:49 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Mon, 25 Oct 2021 18:24:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535227b9f7486c45ef36f9ff074c2ca4a167ee1cdcc38db678360dc4a814f8a7`  
		Last Modified: Mon, 25 Oct 2021 18:28:04 GMT  
		Size: 191.8 MB (191757703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
