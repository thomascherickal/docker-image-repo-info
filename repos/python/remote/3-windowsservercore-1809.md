## `python:3-windowsservercore-1809`

```console
$ docker pull python@sha256:99b5956a19325c1c793aac60043f1c2a01846e115c1c9bfe7c7e37be809e3556
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2452; amd64

### `python:3-windowsservercore-1809` - windows version 10.0.17763.2452; amd64

```console
$ docker pull python@sha256:61fbeda4fbbf42925ae208019dcd2e1db70803b5fb03f9228208da69476de6ab
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2765258240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:248f80a9e4a928bdf5181d5b2d33b850e813a3855794cdb374f2a6e021f4e170`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 07 Jan 2022 22:48:13 GMT
RUN Install update 1809-amd64
# Wed, 12 Jan 2022 05:11:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Jan 2022 06:13:45 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 19 Jan 2022 17:37:16 GMT
ENV PYTHON_VERSION=3.10.2
# Wed, 19 Jan 2022 17:37:18 GMT
ENV PYTHON_RELEASE=3.10.2
# Wed, 19 Jan 2022 17:39:22 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 19 Jan 2022 17:39:24 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 19 Jan 2022 17:39:25 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 19 Jan 2022 17:39:26 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3cb8888cc2869620f57d5d2da64da38f516078c7/public/get-pip.py
# Wed, 19 Jan 2022 17:39:28 GMT
ENV PYTHON_GET_PIP_SHA256=c518250e91a70d7b20cceb15272209a4ded2a0c263ae5776f129e0d9b5674309
# Wed, 19 Jan 2022 17:40:58 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 19 Jan 2022 17:40:59 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:635f15ebd5b486e8a00bf217a0574a29550e5bbf08c1d021e1e308100b2e49b5`  
		Size: 993.9 MB (993898043 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3a70d5fd54e2005efbf590b48700ed40509210354a0d8f3f18c3b444a5325896`  
		Last Modified: Wed, 12 Jan 2022 06:20:33 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ec0edebd1ddbb9c1b3b254bb09452f2077c1a30226af03c61c009222a6c5c1`  
		Last Modified: Wed, 12 Jan 2022 06:21:32 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e48ddbd4426c730811a357801579cf7ca3a198eca6be45a86e113f104fe7e9`  
		Last Modified: Wed, 19 Jan 2022 17:51:57 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac686b3dfb056a1450a9f5efa76c428d8188136a03ff50854e0c8507e08cd894`  
		Last Modified: Wed, 19 Jan 2022 17:51:58 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa359adfef53cfef5c5cb3fdeac9ca1745f14a9f023b6761b4fcb8386abf0469`  
		Last Modified: Wed, 19 Jan 2022 17:52:08 GMT  
		Size: 46.5 MB (46542858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:371a617c978151b8fb0a7175aafb5cb7021117f32a4f50fb1020808d6b87c51a`  
		Last Modified: Wed, 19 Jan 2022 17:51:57 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69bacd15d5baaeccb0e24def5fbe27d83291522b9258d23461c62cbfcb67cfba`  
		Last Modified: Wed, 19 Jan 2022 17:51:54 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f98253beaa0d1c34a10d5119dcd551709fd7dc951bf7ebe7b1c8cc0cd6ba8c4`  
		Last Modified: Wed, 19 Jan 2022 17:51:54 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b42919a9ac89ec714fb22781b005960e0fab85e8bb26e22f1c4f3cafd69d9c4`  
		Last Modified: Wed, 19 Jan 2022 17:51:54 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb57ef4d786de73a8ff2aa99be5e3aae76715bbf26eda499a86ec2759d0cd3b`  
		Last Modified: Wed, 19 Jan 2022 17:51:57 GMT  
		Size: 6.5 MB (6471704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a996d7a4a4f45aacf0072c1966bf68f90dd24740a6d536b0f2be2cb282f8f0`  
		Last Modified: Wed, 19 Jan 2022 17:51:54 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
