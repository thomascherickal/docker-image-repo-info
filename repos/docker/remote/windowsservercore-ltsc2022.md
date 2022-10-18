## `docker:windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:a76fd410786c8e831a8ca7a667e17237136d29a13c4f1583bbbb219ccad3eecc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1129; amd64

### `docker:windowsservercore-ltsc2022` - windows version 10.0.20348.1129; amd64

```console
$ docker pull docker@sha256:777d414b8507576152284279078a4dac22d9987cb0a80152790ecb291c841f77
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2471491387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48092d90a92774b89be7bc6c0d50dec1da28848243d301c93c4777f0eaeae93e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 07 Oct 2022 22:13:48 GMT
RUN Install update 10.0.20348.1129
# Tue, 11 Oct 2022 20:20:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 18:07:47 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 18 Oct 2022 21:16:04 GMT
ENV DOCKER_VERSION=20.10.20
# Tue, 18 Oct 2022 21:16:05 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.20.zip
# Tue, 18 Oct 2022 21:16:50 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ab91661ce2a2a2c14684a2ba0f543a81d7896773f88200b31be0e37c589de38`  
		Size: 979.4 MB (979359717 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:15e15cecc9c7498ee7335091ed603347777bb2f7810e8b701327779faaae1712`  
		Last Modified: Tue, 11 Oct 2022 20:34:44 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb3038ebf46d13f3797c5bef150bfa682c8a25ee893c0ae7b1e9220a0fc1cad`  
		Last Modified: Wed, 12 Oct 2022 18:13:35 GMT  
		Size: 608.0 KB (607995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9676d4fcd2248039c6f80c964c0f0165f6f35e478bdb603c32cd3e3e00e6c57`  
		Last Modified: Tue, 18 Oct 2022 21:19:09 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff89ef16d5c5cbe7f600a44afaba31927c48fb8e8446f8ab83cc3ae5788c4eaf`  
		Last Modified: Tue, 18 Oct 2022 21:19:09 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b231ebbaf4b904e7b1dac1386fc746f8af04d078bb041a5220f80e4c38e88fc1`  
		Last Modified: Tue, 18 Oct 2022 21:19:19 GMT  
		Size: 54.7 MB (54655824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
