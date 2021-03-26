## `jobber:latest`

```console
$ docker pull jobber@sha256:63124190432392d9616d80236a37c3b81bf9a3db610b7746ce3bd9040b2cbe25
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `jobber:latest` - linux; amd64

```console
$ docker pull jobber@sha256:d387ac412b099eb135b0efc68f175e599d53ad72181b881be5a78acc57a51522
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **11.8 MB (11762597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd210e528b5d5c84f8ae3bf344bd57c4163e2765d3b3c48983818a477df93d70`
-	Default Command: `["\/usr\/libexec\/jobberrunner","-u","\/var\/jobber\/1000\/cmd.sock","\/home\/jobberuser\/.jobber"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:43 GMT
ADD file:05adf37fc1a41a31d8e0e0b9371a01161abc0d348adacbc81689a1a34e8fe12d in / 
# Thu, 25 Mar 2021 22:19:43 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 02:48:41 GMT
ENV USERID=1000
# Fri, 26 Mar 2021 02:48:44 GMT
RUN addgroup jobberuser &&     adduser -S -u "${USERID}" -G jobberuser jobberuser &&     mkdir -p "/var/jobber/${USERID}" &&     chown -R jobberuser:jobberuser "/var/jobber/${USERID}"
# Fri, 26 Mar 2021 02:48:44 GMT
ENV JOBBER_VERSION=1.4.4
# Fri, 26 Mar 2021 02:48:44 GMT
ENV JOBBER_SHA256=ec09b2efafff69c91fba2124bf28607209e1c9b50ed834ff444a9d40798aa8d3
# Fri, 26 Mar 2021 02:48:49 GMT
RUN wget -O /tmp/jobber.apk "https://github.com/dshearer/jobber/releases/download/v${JOBBER_VERSION}/jobber-${JOBBER_VERSION}-r0.apk" &&     echo -n "Actual checksum: " && sha256sum /tmp/jobber.apk &&     echo "${JOBBER_SHA256} */tmp/jobber.apk" | sha256sum -c &&     apk add --no-network --no-scripts --allow-untrusted /tmp/jobber.apk &&     rm /tmp/jobber.apk
# Fri, 26 Mar 2021 02:48:49 GMT
COPY --chown=jobberuser:jobberuserfile:c7cc6d32091e7beeac78efd9fe855e36a106902c1177df0f9f6bd2bbe3b8d518 in /home/jobberuser/.jobber 
# Fri, 26 Mar 2021 02:48:52 GMT
RUN chmod 0600 /home/jobberuser/.jobber
# Fri, 26 Mar 2021 02:48:52 GMT
USER jobberuser
# Fri, 26 Mar 2021 02:48:52 GMT
CMD ["/usr/libexec/jobberrunner" "-u" "/var/jobber/1000/cmd.sock" "/home/jobberuser/.jobber"]
```

-	Layers:
	-	`sha256:839b45e0263abc8ab2dc0bfabc91a19947e932ffbd551a93970ea3ee971eadf6`  
		Last Modified: Thu, 25 Mar 2021 22:20:47 GMT  
		Size: 2.8 MB (2815332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847c987c90b1245e08fb05a7c3b19f8be20b01671ff159ebd612f6cb966ae60b`  
		Last Modified: Fri, 26 Mar 2021 02:49:08 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de24dfae73e96a719b9ec5a064efa56c31b907c766d2b69a211aa2beca2666a`  
		Last Modified: Fri, 26 Mar 2021 02:49:10 GMT  
		Size: 8.9 MB (8945465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42a04dfa576f6c19f031415537f9ef4f81927b6b6185898cb049f4d747977aca`  
		Last Modified: Fri, 26 Mar 2021 02:49:07 GMT  
		Size: 235.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7024523f4aa43cbf728a24f6bd31bc43f9b3f9e1b241a1587b6d34be4261102`  
		Last Modified: Fri, 26 Mar 2021 02:49:07 GMT  
		Size: 234.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
