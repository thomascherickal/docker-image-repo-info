## `nats:windowsservercore-ltsc2016`

```console
$ docker pull nats@sha256:1a4671a9526fb6ede83b18c71177d3af3cf4fcc206e12af3ab5d17dbe9aaf52f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64

### `nats:windowsservercore-ltsc2016` - windows version 10.0.14393.3568; amd64

```console
$ docker pull nats@sha256:2eac3c1b323e0a2404c52f47267585d613b0283a5813550b302385359d03105a
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5743565301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3850b6ab7edb6d2c776657774444acdc4d40c667e3d2d752fa536ce0f90f2d6`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 13:38:31 GMT
ENV NATS_DOCKERIZED=1
# Wed, 18 Mar 2020 13:38:32 GMT
ENV NATS_SERVER=2.1.4
# Wed, 18 Mar 2020 13:38:33 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.4/nats-server-v2.1.4-windows-amd64.zip
# Wed, 18 Mar 2020 13:39:42 GMT
RUN Set-PSDebug -Trace 2
# Wed, 18 Mar 2020 13:41:30 GMT
RUN Write-Host ('downloading from {0}' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*
# Wed, 18 Mar 2020 13:41:31 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 18 Mar 2020 13:41:32 GMT
EXPOSE 4222 6222 8222
# Wed, 18 Mar 2020 13:41:33 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 18 Mar 2020 13:41:34 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddde0325982310255792cba68184203cd656b044bf4f46ab5c1ebf779122527`  
		Last Modified: Wed, 18 Mar 2020 13:42:12 GMT  
		Size: 1.1 KB (1135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c08b5e9143a48c4d197e5ab6e90d4a24df1f9f046acfffe8d3c033801e1409`  
		Last Modified: Wed, 18 Mar 2020 13:42:12 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795ae1863ef93b612e9e360fc0d0ea435881cd108b2e5f224b3b7d0361d37b3b`  
		Last Modified: Wed, 18 Mar 2020 13:42:12 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8825d20073f1d69326e9c05a45176f93b474c93749fbd4d52994e205f81b431b`  
		Last Modified: Wed, 18 Mar 2020 13:42:13 GMT  
		Size: 5.4 MB (5383002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4411a97b731ba87efc271d3f27f6742dabc2f611e9ee06d092df3103968637`  
		Last Modified: Wed, 18 Mar 2020 13:42:20 GMT  
		Size: 9.4 MB (9411571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f962640772bb86ec8dd6df40d872dfd1731f275102828598d34d815e8a4c4d`  
		Last Modified: Wed, 18 Mar 2020 13:42:09 GMT  
		Size: 1.7 KB (1673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c249fbbace74a9b9605df64c2fa32b48292b2e3c669d6767354453b81ba460c7`  
		Last Modified: Wed, 18 Mar 2020 13:42:09 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fab83c2144f7317f188eeb048d9553da61fd5061302b0db0cdec39869dc1f7b`  
		Last Modified: Wed, 18 Mar 2020 13:42:09 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6fe2fceefa927b9e09df57f083f11b317238239c2a9cb815617ad1200abf388`  
		Last Modified: Wed, 18 Mar 2020 13:42:09 GMT  
		Size: 1.1 KB (1145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
