## `amazoncorretto:18-alpine3.13-jdk`

```console
$ docker pull amazoncorretto@sha256:0976aaaca83bccf799624291bce6773a5306e148671ce220d6068ec6e5d09688
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `amazoncorretto:18-alpine3.13-jdk` - linux; amd64

```console
$ docker pull amazoncorretto@sha256:404ed255b0e7fe132ec43e81c0a0a34e506cb00c2a3ddecc292d01bfd0f75b98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **195.7 MB (195680150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e35584525f3e20934f06281b376bc1ecbd1d4683115b6fed7485559eb2729d3a`
-	Default Command: `["\/bin\/sh"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:26 GMT
ADD file:e15461ac94648d9599df6304a53587fc8bfceaf6e111ee5917860e95ed9e751c in / 
# Tue, 19 Jul 2022 22:20:26 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 22:40:01 GMT
ARG version=18.0.2.9.1
# Tue, 19 Jul 2022 22:40:07 GMT
# ARGS: version=18.0.2.9.1
RUN wget -O /THIRD-PARTY-LICENSES-20200824.tar.gz https://corretto.aws/downloads/resources/licenses/alpine/THIRD-PARTY-LICENSES-20200824.tar.gz &&     echo "82f3e50e71b2aee21321b2b33de372feed5befad6ef2196ddec92311bc09becb  /THIRD-PARTY-LICENSES-20200824.tar.gz" | sha256sum -c - &&     tar x -ovzf THIRD-PARTY-LICENSES-20200824.tar.gz &&     rm -rf THIRD-PARTY-LICENSES-20200824.tar.gz &&     wget -O /etc/apk/keys/amazoncorretto.rsa.pub https://apk.corretto.aws/amazoncorretto.rsa.pub &&     SHA_SUM="6cfdf08be09f32ca298e2d5bd4a359ee2b275765c09b56d514624bf831eafb91" &&     echo "${SHA_SUM}  /etc/apk/keys/amazoncorretto.rsa.pub" | sha256sum -c - &&     echo "https://apk.corretto.aws" >> /etc/apk/repositories &&     apk add --no-cache amazon-corretto-18=$version-r0
# Tue, 19 Jul 2022 22:40:08 GMT
ENV LANG=C.UTF-8
# Tue, 19 Jul 2022 22:40:08 GMT
ENV JAVA_HOME=/usr/lib/jvm/default-jvm
# Tue, 19 Jul 2022 22:40:08 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/lib/jvm/default-jvm/bin
```

-	Layers:
	-	`sha256:627fad6f28f79c3907ad18a4399be4d810c0e1bb503fe3712217145c555b9d2f`  
		Last Modified: Tue, 19 Jul 2022 22:21:04 GMT  
		Size: 2.8 MB (2819330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a579b47768be7cf964521b4ccf9ae6a8b572ef21b2841ba2840099c088b362a`  
		Last Modified: Tue, 19 Jul 2022 22:49:10 GMT  
		Size: 192.9 MB (192860820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
