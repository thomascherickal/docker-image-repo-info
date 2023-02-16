## `nats:windowsservercore`

```console
$ docker pull nats@sha256:65c1926af840363eb9f7167d86a3c16835c08bc50ca46734397db7741c101218
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.4010; amd64

### `nats:windowsservercore` - windows version 10.0.17763.4010; amd64

```console
$ docker pull nats@sha256:79bd62dbbae09c0dd17cae39d8a2aede262b06de814be6e7670731d9cb6fc5c1
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.0 GB (1968801824 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c081257ecbd4944adc27bd0b5f6ae5e2ac35f0cf51520148c335d6145259a6a`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Tue, 07 Feb 2023 10:44:53 GMT
RUN Install update 10.0.17763.4010
# Thu, 16 Feb 2023 00:42:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 16 Feb 2023 02:04:44 GMT
ENV NATS_DOCKERIZED=1
# Thu, 16 Feb 2023 02:04:45 GMT
ENV NATS_SERVER=2.9.14
# Thu, 16 Feb 2023 02:04:46 GMT
ENV NATS_SERVER_DOWNLOAD=https://github.com/nats-io/nats-server/releases/download/v2.9.14/nats-server-v2.9.14-windows-amd64.zip
# Thu, 16 Feb 2023 02:04:47 GMT
ENV NATS_SERVER_SHASUM=b47ca5d88b1a74934145aba3afd6a3b0eee0e543638000cee82b468b8dfbcb3c
# Thu, 16 Feb 2023 02:05:59 GMT
RUN Set-PSDebug -Trace 2
# Thu, 16 Feb 2023 02:07:24 GMT
RUN Write-Host ('downloading from {0} ...' -f $env:NATS_SERVER_DOWNLOAD); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:NATS_SERVER_DOWNLOAD -OutFile nats.zip; 		Write-Host ('verifying sha256 ({0}) ...' -f $env:NATS_SERVER_SHASUM); 	if ((Get-FileHash nats.zip -Algorithm sha256).Hash -ne $env:NATS_SERVER_SHASUM) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 	Write-Host 'extracting nats.zip'; 	Expand-Archive -Path 'nats.zip' -DestinationPath .; 		Write-Host 'copying binary'; 	Copy-Item nats-server-v*/nats-server.exe -Destination C:\\nats-server.exe; 		Write-Host 'cleaning up'; 	Remove-Item -Force nats.zip; 	Remove-Item -Recurse -Force nats-server-v*; 		Write-Host 'complete.';
# Thu, 16 Feb 2023 02:07:25 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in C:\nats-server.conf 
# Thu, 16 Feb 2023 02:07:26 GMT
EXPOSE 4222 6222 8222
# Thu, 16 Feb 2023 02:07:27 GMT
ENTRYPOINT ["C:\\nats-server.exe"]
# Thu, 16 Feb 2023 02:07:27 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f77c707e813c8220ab3c92b6eb7b445ee0b1a485686ff62014ae32c17d2b1b6`  
		Last Modified: Thu, 16 Feb 2023 00:29:31 GMT  
		Size: 255.0 MB (255014079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531f6c3ad9784fc2870ea5ca08c4adccd9318602ed534d822e12b8b658a7b0b6`  
		Last Modified: Thu, 16 Feb 2023 01:37:30 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724509671085dbea52985b930945ecf6cb7694ecee9924bc0226a51a4e01d8a5`  
		Last Modified: Thu, 16 Feb 2023 02:08:17 GMT  
		Size: 1.3 KB (1324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c57383dcb3414d845f4527f621e03111d1d21466c7f8a450b965347f4783ae`  
		Last Modified: Thu, 16 Feb 2023 02:08:15 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d16e9ec785328185eb999dbfaff65594e87082753146845209f6ae34788e5fb`  
		Last Modified: Thu, 16 Feb 2023 02:08:15 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d67059b5bac5befe7ea736a46333a3fdeda618257602fa047ad07a69b36559c`  
		Last Modified: Thu, 16 Feb 2023 02:08:15 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4538cb8ed4700f33db1c6b84b45e353e9978f3edb2b073163af177c8db8ce45b`  
		Last Modified: Thu, 16 Feb 2023 02:08:15 GMT  
		Size: 483.0 KB (482966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa50a7f3068bb6f22184b0acd7e4f0768d04c090410409c6e2505062c167cb62`  
		Last Modified: Thu, 16 Feb 2023 02:08:14 GMT  
		Size: 5.3 MB (5348523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5048e889f3efca79f9657e7d3c99f3b4328422e2f0b1a2ff2cf828ce0604bf1`  
		Last Modified: Thu, 16 Feb 2023 02:08:13 GMT  
		Size: 1.9 KB (1899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daff995efe19f6f8578c54ca78a31af8b8d68c8621ff813f7a538a823b270cf2`  
		Last Modified: Thu, 16 Feb 2023 02:08:13 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8a75777236872d7bb2f94eebb1d7351638b0b23f4df09f558d44fe6e0efc79c`  
		Last Modified: Thu, 16 Feb 2023 02:08:13 GMT  
		Size: 1.3 KB (1345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918d68bc0df2dee65e560db5a14091cc62492f0e0bf0b8fc4ce134c69b1d77a0`  
		Last Modified: Thu, 16 Feb 2023 02:08:13 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
