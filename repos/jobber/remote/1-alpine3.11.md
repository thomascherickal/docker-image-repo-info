## `jobber:1-alpine3.11`

```console
$ docker pull jobber@sha256:9007ad3980ebd786be63107ec8d746f44b4aa40ca6c93376bba4f80280b31049
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jobber:1-alpine3.11` - linux; amd64

```console
$ docker pull jobber@sha256:3920b2a0597bb70e87e9f89df1e37dd0f469b85a1cb4de9da4d1555b7b647603
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.8 MB (11762629 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3189acccb914ea861d3710b7665671fab35eafdbbb3b26f646c9867490bf40c`
-	Default Command: `["\/usr\/libexec\/jobberrunner","-u","\/var\/jobber\/1000\/cmd.sock","\/home\/jobberuser\/.jobber"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:19 GMT
ADD file:c744c1dc3da4145771e66d90e2e97a4f7fb702e5e07cf4e766ee0792cf161d92 in / 
# Wed, 31 Mar 2021 20:10:19 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 14:24:36 GMT
ENV USERID=1000
# Thu, 01 Apr 2021 14:24:37 GMT
RUN addgroup jobberuser &&     adduser -S -u "${USERID}" -G jobberuser jobberuser &&     mkdir -p "/var/jobber/${USERID}" &&     chown -R jobberuser:jobberuser "/var/jobber/${USERID}"
# Thu, 01 Apr 2021 14:24:37 GMT
ENV JOBBER_VERSION=1.4.4
# Thu, 01 Apr 2021 14:24:38 GMT
ENV JOBBER_SHA256=ec09b2efafff69c91fba2124bf28607209e1c9b50ed834ff444a9d40798aa8d3
# Thu, 01 Apr 2021 14:24:40 GMT
RUN wget -O /tmp/jobber.apk "https://github.com/dshearer/jobber/releases/download/v${JOBBER_VERSION}/jobber-${JOBBER_VERSION}-r0.apk" &&     echo -n "Actual checksum: " && sha256sum /tmp/jobber.apk &&     echo "${JOBBER_SHA256} */tmp/jobber.apk" | sha256sum -c &&     apk add --no-network --no-scripts --allow-untrusted /tmp/jobber.apk &&     rm /tmp/jobber.apk
# Thu, 01 Apr 2021 14:24:40 GMT
COPY --chown=jobberuser:jobberuserfile:c7cc6d32091e7beeac78efd9fe855e36a106902c1177df0f9f6bd2bbe3b8d518 in /home/jobberuser/.jobber 
# Thu, 01 Apr 2021 14:24:41 GMT
RUN chmod 0600 /home/jobberuser/.jobber
# Thu, 01 Apr 2021 14:24:42 GMT
USER jobberuser
# Thu, 01 Apr 2021 14:24:42 GMT
CMD ["/usr/libexec/jobberrunner" "-u" "/var/jobber/1000/cmd.sock" "/home/jobberuser/.jobber"]
```

-	Layers:
	-	`sha256:9b794450f7b6db7c944ba1f4161edb68cb535052fe7db8ac06e613516c4a658d`  
		Last Modified: Wed, 31 Mar 2021 20:11:14 GMT  
		Size: 2.8 MB (2815346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e617a45e437a950c0af202ef4f56187d3f54cfe98bfc09dc48e2db0e86ba4cdf`  
		Last Modified: Thu, 01 Apr 2021 14:24:53 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c75bed0074aaeb96fce9807a641c64478ece4444facf80f50fbccb4c01dbfab`  
		Last Modified: Thu, 01 Apr 2021 14:24:55 GMT  
		Size: 8.9 MB (8945482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dec65f664cadd6f4f7e93de247c31992bb9a16d266c0ca0f30b07bf04f16408`  
		Last Modified: Thu, 01 Apr 2021 14:24:53 GMT  
		Size: 236.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132768e29d5b895b9f7abab73e7cfaec4d0367a1acf71aabbb6bdbe8ed29033a`  
		Last Modified: Thu, 01 Apr 2021 14:24:53 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
