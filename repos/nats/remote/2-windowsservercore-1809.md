## `nats:2-windowsservercore-1809`

```console
$ docker pull nats@sha256:68052566a345b1974727afb0e13ccf5da8cd92efabede8c67f188abaabecdac9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `nats:2-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull nats@sha256:1c83509a0dd49bb818407142b5595766fc8cadb59834e72c0a91deaea371ff34
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2369206825 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06a6b490bf0f236facc1bf15bf5fbab8a4741401eb02c00e2bf0f129dd66c20d`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Sep 2020 13:15:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_DOCKERIZED=1
# Wed, 09 Sep 2020 17:10:34 GMT
ENV NATS_SERVER=2.1.8
# Wed, 09 Sep 2020 17:10:35 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.1.8/nats-server-v2.1.8-windows-amd64.zip
# Wed, 09 Sep 2020 17:10:35 GMT
ENV GIT_DOWNLOAD_SHA256=198246c4bc9c16a8d9866ab665ba91bfb31464b9a08f08108337b10ed4c23478
# Wed, 09 Sep 2020 17:11:05 GMT
RUN Set-PSDebug -Trace 2
# Wed, 09 Sep 2020 17:12:10 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Wed, 09 Sep 2020 17:12:11 GMT
COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Wed, 09 Sep 2020 17:12:12 GMT
EXPOSE 4222 6222 8222
# Wed, 09 Sep 2020 17:12:13 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Wed, 09 Sep 2020 17:12:14 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1df31adcc7026c3bf0cb32832a3f307dd6e1e54b8b3e050f8a73b5caee674d88`  
		Last Modified: Wed, 09 Sep 2020 16:48:51 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a005485001c0802bc2ee93661375bfb4c868e16c3f5678debf00f29a8bb26386`  
		Last Modified: Wed, 09 Sep 2020 17:16:08 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662e6fbc5f9e16fc0afc4d05927cd1e64bfa92f69d228567abe407bb72908aaf`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7151925f65e3cf12e20bc6f6aa94dfb90b475195bea0a8bd3c8d70d21fe6e7`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf309bd49456f53f290cc9143ca63dc647713cb7981d22d61d7f8b18548b8ae`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fd4c97d4d46deef398e38f156ba05f404a8de7e7f7915b45a96e1b84c98e2e`  
		Last Modified: Wed, 09 Sep 2020 17:16:11 GMT  
		Size: 4.8 MB (4784097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39896e9d43e963384628807bede8a7bea2735860d8797978d74cdccb2db3cccc`  
		Last Modified: Wed, 09 Sep 2020 17:16:06 GMT  
		Size: 13.1 MB (13139733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303f12072d6a77ef8f3b35b86cd6fd3a37c88fdd85e2a20d6946ad7fdb5678b4`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.7 KB (1705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02cf56909eff26727cabe26c37adb7b07aa76875550f66e267c0e9044d8f19c7`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be0c7ccbe6779b4f737d7987f4246dc066853208e9957364e0ea8e0d4ee07b47`  
		Last Modified: Wed, 09 Sep 2020 17:16:04 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a250cb3a50140ec9efe6f52457ea634df38df6babd373210cf8c5abb888f7a29`  
		Last Modified: Wed, 09 Sep 2020 17:16:03 GMT  
		Size: 1.2 KB (1168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
