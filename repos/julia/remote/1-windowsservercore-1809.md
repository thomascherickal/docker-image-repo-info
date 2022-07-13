## `julia:1-windowsservercore-1809`

```console
$ docker pull julia@sha256:fe35d3bbafd7b7fa3cb2d21565aab8cf295d86fc32fe5fbed97f59bd3f65bd47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3165; amd64

### `julia:1-windowsservercore-1809` - windows version 10.0.17763.3165; amd64

```console
$ docker pull julia@sha256:8b421bdb04b44bffb9d2f9134e87dabf556dad631b77591da93c7c355e98697e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2816994947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c3cfa5d6f8b359be0b1eca14296a62836517203a6884d50b44fc3029d3b54a`
-	Default Command: `["julia"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Wed, 06 Jul 2022 22:37:15 GMT
RUN Install update 10.0.17763.3165
# Tue, 12 Jul 2022 19:32:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jul 2022 14:27:42 GMT
ENV JULIA_VERSION=1.7.3
# Wed, 13 Jul 2022 14:27:43 GMT
ENV JULIA_URL=https://julialang-s3.julialang.org/bin/winnt/x64/1.7/julia-1.7.3-win64.exe
# Wed, 13 Jul 2022 14:27:44 GMT
ENV JULIA_SHA256=ef5915eaf35bb71359072e8c41f84fa73f1059fecb198e7fc838270d4ba5bbae
# Wed, 13 Jul 2022 14:30:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JULIA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JULIA_URL -OutFile 'julia.exe'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:JULIA_SHA256); 	if ((Get-FileHash julia.exe -Algorithm sha256).Hash -ne $env:JULIA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -Wait -NoNewWindow 		-FilePath '.\julia.exe' 		-ArgumentList @( 			'/SILENT', 			'/DIR=C:\julia' 		); 		Write-Host 'Removing ...'; 	Remove-Item julia.exe -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\julia\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("julia --version") ...'; 	julia --version; 		Write-Host 'Complete.'
# Wed, 13 Jul 2022 14:30:06 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7aca8de30754f19fe03ee4c21eed0762efb5e91bf684b0cc36cc92b2af13446d`  
		Size: 794.9 MB (794877652 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:912efe6370f7047e630e1f70d9201e3143571e3ed1fe50a1e61754d2d536ea95`  
		Last Modified: Tue, 12 Jul 2022 20:21:55 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bebb8c27e8eecf971d3699afde71c95c7fac805c0084c901b2a3761dcf7b1d28`  
		Last Modified: Wed, 13 Jul 2022 14:38:00 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d6935ffb4853a580c27e0b8ebc1ee35e4bede87ca36647623ab780ed9bc9b7`  
		Last Modified: Wed, 13 Jul 2022 14:38:01 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00d84dc104861e3f2e614a29110c7ffef9dbd16b4e4cc2af25f31eb386ef9195`  
		Last Modified: Wed, 13 Jul 2022 14:38:00 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bfd15c2f57ceb1b396af7d24ea695b743c1b44cf715c50c6aa99afc8b88bda`  
		Last Modified: Wed, 13 Jul 2022 14:38:29 GMT  
		Size: 144.9 MB (144944112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6709a8297df91b521cbc03f8d4f777aae7dbbc7d89ee2720cd7f83e05c00d468`  
		Last Modified: Wed, 13 Jul 2022 14:38:00 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
