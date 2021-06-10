## `caddy:2-windowsservercore-ltsc2016`

```console
$ docker pull caddy@sha256:f07a9aef54a1c73076c58ba7037c8840b67601723e6dbf534878e515d02f519d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4467; amd64

### `caddy:2-windowsservercore-ltsc2016` - windows version 10.0.14393.4467; amd64

```console
$ docker pull caddy@sha256:e7e7af29e7917229552a0c802147dba99fb7a1427b84296a2c60ea7e19cbcb0c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6278267906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7184db699efd0a2ce0077179784cc7277e5faa7d07534ea1ce32d61d7f46ebc`
-	Default Command: `["caddy","run","--config","\/etc\/caddy\/Caddyfile","--adapter","caddyfile"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 06 Jun 2021 15:37:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Jun 2021 12:41:37 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Jun 2021 20:11:27 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     mkdir /config;     mkdir /data;     mkdir /etc/caddy;     mkdir /usr/share/caddy;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/config/Caddyfile"         -OutFile "/etc/caddy/Caddyfile";     Invoke-WebRequest         -Uri "https://github.com/caddyserver/dist/raw/a8ef04588bf34a9523b76794d601c6e9cb8e31d3/welcome/index.html"         -OutFile "/usr/share/caddy/index.html"
# Wed, 09 Jun 2021 20:11:30 GMT
ENV CADDY_VERSION=v2.4.1
# Wed, 09 Jun 2021 20:13:06 GMT
RUN [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     Invoke-WebRequest         -Uri "https://github.com/caddyserver/caddy/releases/download/v2.4.1/caddy_2.4.1_windows_amd64.zip"         -OutFile "/caddy.zip";     if (!(Get-FileHash -Path /caddy.zip -Algorithm SHA512).Hash.ToLower().Equals('67655d9a62e508753bea183e9fbfd3b890b280f16c8ef416b3524fc7638d38caa58390fe91378eba058123a4e3007d2e6949ad626ee15c6103ed34daccd06e46')) { exit 1; };     Expand-Archive -Path "/caddy.zip" -DestinationPath "/" -Force;     Remove-Item "/caddy.zip" -Force
# Wed, 09 Jun 2021 20:13:09 GMT
ENV XDG_CONFIG_HOME=c:/config
# Wed, 09 Jun 2021 20:13:11 GMT
ENV XDG_DATA_HOME=c:/data
# Wed, 09 Jun 2021 20:13:15 GMT
VOLUME [c:/config]
# Wed, 09 Jun 2021 20:13:18 GMT
VOLUME [c:/data]
# Wed, 09 Jun 2021 20:13:20 GMT
LABEL org.opencontainers.image.version=v2.4.1
# Wed, 09 Jun 2021 20:13:23 GMT
LABEL org.opencontainers.image.title=Caddy
# Wed, 09 Jun 2021 20:13:25 GMT
LABEL org.opencontainers.image.description=a powerful, enterprise-ready, open source web server with automatic HTTPS written in Go
# Wed, 09 Jun 2021 20:13:28 GMT
LABEL org.opencontainers.image.url=https://caddyserver.com
# Wed, 09 Jun 2021 20:13:30 GMT
LABEL org.opencontainers.image.documentation=https://caddyserver.com/docs
# Wed, 09 Jun 2021 20:13:32 GMT
LABEL org.opencontainers.image.vendor=Light Code Labs
# Wed, 09 Jun 2021 20:13:35 GMT
LABEL org.opencontainers.image.licenses=Apache-2.0
# Wed, 09 Jun 2021 20:13:37 GMT
LABEL org.opencontainers.image.source=https://github.com/caddyserver/caddy-docker
# Wed, 09 Jun 2021 20:13:40 GMT
EXPOSE 80
# Wed, 09 Jun 2021 20:13:42 GMT
EXPOSE 443
# Wed, 09 Jun 2021 20:13:45 GMT
EXPOSE 2019
# Wed, 09 Jun 2021 20:14:40 GMT
RUN caddy version
# Wed, 09 Jun 2021 20:14:43 GMT
CMD ["caddy" "run" "--config" "/etc/caddy/Caddyfile" "--adapter" "caddyfile"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2f52abeee6d6f4a925ad418b5e6200d4fca9bf92834ffc918b8bbaccd34251db`  
		Size: 2.2 GB (2195741359 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c82e82e95dbad4ccc260b42e03767eb07222e2f00ec57a69b3c87b17da1d2fd3`  
		Last Modified: Wed, 09 Jun 2021 13:04:25 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a28e390d3b8e7b9369b102914eaee6e1fa0d14eb258b628be67f99f32f06f81`  
		Last Modified: Wed, 09 Jun 2021 20:20:01 GMT  
		Size: 357.4 KB (357370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82f7f07987f083e935103f83e47894b93aceaf05d1ded81dd09eb0bc3c8e45af`  
		Last Modified: Wed, 09 Jun 2021 20:20:01 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e65ddfdcdd60907208873b2a532cc58bc0f57d144430cef2c7630e80e4fd1e`  
		Last Modified: Wed, 09 Jun 2021 20:20:05 GMT  
		Size: 11.9 MB (11896985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e58e4679b7ef7e1b9d82f44a6b5055c6916801193550bcce3ce390851224c736`  
		Last Modified: Wed, 09 Jun 2021 20:20:00 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4107d803623512ea83de929509cc68f334261f2018c60bde60a99eadd0c2b179`  
		Last Modified: Wed, 09 Jun 2021 20:20:00 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f757538ddb020d145715a4890594958e741fe98366f1a58314361e5a8a3487`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462510ee9cb1c642e2804f8f607f02ccc5c31b63c956b9394bf38c5041b10d8b`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e87709f8365472aa7278651dacfc7eee93b24859a494cf6904b4f7ce80df0a`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5439b862b8218f1d7e0e0269efdbed614475ffbdcbaac06a3953f80b07677a1a`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1950c17917c025587fa23872145ee00eaaa11939dc87314c1aa74119db642d`  
		Last Modified: Wed, 09 Jun 2021 20:19:58 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84164685053ad8b12a46e198ec2e93143d1df956bbbd4af76c88d0f549031c60`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103b7e93d2e2faefef7bd14bc00910442ce8da843f4fb726e2dba2d97752ddc9`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046d1e0cd75d46944ff833afe00c5dc9835ec1eb72876965a98a1488778910a6`  
		Last Modified: Wed, 09 Jun 2021 20:19:56 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593a0ce075f6e5e07785dd7cd14aa1c274339da4d6f80495f0d1a85fabdef5db`  
		Last Modified: Wed, 09 Jun 2021 20:19:55 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f14f5cdc43c91f65e6c5879691adc6e392d353807b27465a9b270fe7a06da51c`  
		Last Modified: Wed, 09 Jun 2021 20:19:55 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd488f5f58644d68e5103098932448a58d05a716861b26bf33376e75ad27e61`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c218cc3caa4b354c536ad99d30753a6eb41c52a58c52aafc0655a8482382a07`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3dad29a1e0241680f68697c2b0dbca8e85d0084faef4bdd3e66c8294be80671`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeda652af05f03b2ec029aa5caa6b49d533546fa8347f5b1db003e8a83a7c30`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 260.8 KB (260840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9779c5588bf525e972d3b02ecaeeee32f3939ef8d54e8a16c52e0e62804e2e42`  
		Last Modified: Wed, 09 Jun 2021 20:19:53 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
