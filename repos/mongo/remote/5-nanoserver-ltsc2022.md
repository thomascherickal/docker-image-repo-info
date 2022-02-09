## `mongo:5-nanoserver-ltsc2022`

```console
$ docker pull mongo@sha256:4b4c7666aa2be551cd5f6c4a4e8d989ae96c597f6b0a4dae6146f043a24cc288
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.524; amd64

### `mongo:5-nanoserver-ltsc2022` - windows version 10.0.20348.524; amd64

```console
$ docker pull mongo@sha256:9b74de0a35f4e4b6aa0263597026863e12941e14501f4db19092298bbd2f3496
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **420.3 MB (420289332 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90ae448e1bcb06fcdaf9aeb069e84fc30c64a2948876d6ddf3ebdd837635df93`
-	Default Command: `["mongod","--bind_ip_all"]`
-	`SHELL`: `["cmd","\/S","\/C"]`

```dockerfile
# Tue, 01 Feb 2022 02:25:40 GMT
RUN Apply image ltsc2022-amd64
# Wed, 09 Feb 2022 13:48:34 GMT
SHELL [cmd /S /C]
# Wed, 09 Feb 2022 16:58:27 GMT
USER ContainerAdministrator
# Wed, 09 Feb 2022 16:58:40 GMT
RUN setx /m PATH "C:\mongodb\bin;%PATH%"
# Wed, 09 Feb 2022 16:58:41 GMT
USER ContainerUser
# Wed, 09 Feb 2022 16:58:43 GMT
COPY multi:9a4a91c322ba6325a22891e3a40eb7306a49c53e11d5828931f2326770a3f548 in C:\Windows\System32\ 
# Wed, 09 Feb 2022 16:58:43 GMT
ENV MONGO_VERSION=5.0.6
# Wed, 09 Feb 2022 17:00:13 GMT
COPY dir:8054396aef21c43e8eb1e82c0d52daca301fb548900656fb893eece57b5d6e88 in C:\mongodb 
# Wed, 09 Feb 2022 17:00:24 GMT
RUN mongo --version && mongod --version
# Wed, 09 Feb 2022 17:00:25 GMT
VOLUME [C:\data\db C:\data\configdb]
# Wed, 09 Feb 2022 17:00:26 GMT
EXPOSE 27017
# Wed, 09 Feb 2022 17:00:27 GMT
CMD ["mongod" "--bind_ip_all"]
```

-	Layers:
	-	`sha256:3ab33c1d9cc1eaef56d5617b87373ead45d8a4ff7ab7da384afe612ba569a524`  
		Size: 117.5 MB (117457656 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d52811c4b439c00c93423790e004fc266374135015625d93ffb80def500d7b64`  
		Last Modified: Wed, 09 Feb 2022 14:34:32 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738d5c8c4d24058e48377eb28f6ef1d424c37245dfe1b8cd3b15a5941ba34f52`  
		Last Modified: Wed, 09 Feb 2022 17:38:27 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0bd82a040e4b2e88fb7e59cad10e89c4218dad38a64e4cd9b2696cc1c462623`  
		Last Modified: Wed, 09 Feb 2022 17:38:25 GMT  
		Size: 96.4 KB (96365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac06803457c694043839f4f9d4b86bccda6fdb424a063bcdf4f283c2dd033a0`  
		Last Modified: Wed, 09 Feb 2022 17:38:25 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b577e51ee1e45c3fd8b9d69780861cf94f733dc1189e89bf1e93b9609444328`  
		Last Modified: Wed, 09 Feb 2022 17:38:25 GMT  
		Size: 263.5 KB (263496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc5c6809f27379caf422726a19c90ffccfd1fd7f79f0279399a6b0e0274e2ad`  
		Last Modified: Wed, 09 Feb 2022 17:38:25 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:554ce8d83bd63b4181700b8abecf170519a85e0dcf5d11cee7b2c67bc0b2d4eb`  
		Last Modified: Wed, 09 Feb 2022 17:43:57 GMT  
		Size: 302.4 MB (302387781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76ac0820f81a37d1818e79cb10d563ab30945e793cc9124508905263ae0ed6a`  
		Last Modified: Wed, 09 Feb 2022 17:38:23 GMT  
		Size: 75.9 KB (75902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a49672405f1ee3030b225b03a7118e37065b09295026b9fdd094568de1bda80`  
		Last Modified: Wed, 09 Feb 2022 17:38:23 GMT  
		Size: 1.2 KB (1177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4839d9433c6115bf45d57b8d4b8cfd76385d294a7ad49a71666db57aeb26bc3d`  
		Last Modified: Wed, 09 Feb 2022 17:38:23 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edab9728e0f782a651356784ea8642d3ae0daf1408bee20bf30a40cee229790b`  
		Last Modified: Wed, 09 Feb 2022 17:38:23 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
