## `hylang:python3.9-windowsservercore-1809`

```console
$ docker pull hylang@sha256:a3fb05b5874d1d73362ff6c163f43c7966d821fb33a4a6a3b4c6a04d7678c501
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1879; amd64

### `hylang:python3.9-windowsservercore-1809` - windows version 10.0.17763.1879; amd64

```console
$ docker pull hylang@sha256:007bcfaafed28b5122ca65ace7fbfe5de3425e51098256c81aad804cb3e7b500
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2531584633 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1657f92ffcd10d485f8fa5f0f4fa2ebb014d25adb9c7c4b6020b13fdb435fa1`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 09 Apr 2021 20:34:41 GMT
RUN Install update 1809-amd64
# Wed, 14 Apr 2021 12:09:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 12:14:23 GMT
ENV PYTHONIOENCODING=UTF-8
# Tue, 04 May 2021 17:21:42 GMT
ENV PYTHON_VERSION=3.9.5
# Tue, 04 May 2021 17:21:43 GMT
ENV PYTHON_RELEASE=3.9.5
# Tue, 04 May 2021 17:23:16 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Tue, 04 May 2021 17:23:17 GMT
ENV PYTHON_PIP_VERSION=21.1.1
# Tue, 04 May 2021 17:23:18 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1954f15b3f102ace496a34a013ea76b061535bd2/public/get-pip.py
# Tue, 04 May 2021 17:23:19 GMT
ENV PYTHON_GET_PIP_SHA256=f499d76e0149a673fb8246d88e116db589afbd291739bd84f2cd9a7bca7b6993
# Tue, 04 May 2021 17:24:07 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 04 May 2021 17:24:08 GMT
CMD ["python"]
# Tue, 04 May 2021 17:57:14 GMT
ENV HY_VERSION=1.0a1
# Tue, 04 May 2021 17:57:49 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Tue, 04 May 2021 17:57:49 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:399f118dfaa9a753e98d128238b944432c7bcabea88a2998a6efbbece28ed303`  
		Size: 751.4 MB (751421005 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:106dbf3373fce4f0ba5e00ad54824c597f2894605fa7d8ef446ad7ea3b97449f`  
		Last Modified: Wed, 14 Apr 2021 12:58:04 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc61c4265bfe314fb772d57da4c3023d46cacdbdab9bb6fd5c475f11696dbab`  
		Last Modified: Wed, 14 Apr 2021 16:38:19 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45f34a407781f608740710864eb728c2d66e1c64526d8356b1e86d079c73c30`  
		Last Modified: Tue, 04 May 2021 17:38:42 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e65d6b77b51e1d18d4f858472d376d5ba83c005f4bef4aa51d1ba50515c0e4`  
		Last Modified: Tue, 04 May 2021 17:38:42 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ecf8dbac8a49bdcff41c544d3d36dc05c1fcfc05e41fa539001a2c20a37df0b`  
		Last Modified: Tue, 04 May 2021 17:38:49 GMT  
		Size: 54.4 MB (54390734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1c69368e2d9bcc5fa7b86a2f2710476d9b3b354cb2c9f4018f2a1424f2b648e`  
		Last Modified: Tue, 04 May 2021 17:38:39 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee740df76ca2b1e59a023ffdf5a40503bb4a66797d7729499c2fadc33f505fa`  
		Last Modified: Tue, 04 May 2021 17:38:40 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d87e8ff65e2e70f6b451fc493bc563d8530d8066683d78c6f0d66efb2c19f3`  
		Last Modified: Tue, 04 May 2021 17:38:39 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4874dc8b7e47dd039ae00f9c6d91e0ba3a3ec2c97e383e65f78c1b43ae084eb`  
		Last Modified: Tue, 04 May 2021 17:38:41 GMT  
		Size: 6.2 MB (6217589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5578e5b8480d834c09c1cd5ec33311bca9f936000ddb048a3bca7c3452fa5a10`  
		Last Modified: Tue, 04 May 2021 17:38:39 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3d4d03ee9378632f9905c6473d3e6ba6ae5818ad039e02410b924dbb397ae3d`  
		Last Modified: Tue, 04 May 2021 18:05:19 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41595f832ac7c2304480cb9cad7e4f97c508672907f5fea39409c052dd63faa5`  
		Last Modified: Tue, 04 May 2021 18:05:20 GMT  
		Size: 1.2 MB (1208392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81285d798f1ccb5f986727eaf8420c2fc724a9c39f719919797c5f6759cf4c5`  
		Last Modified: Tue, 04 May 2021 18:05:19 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
