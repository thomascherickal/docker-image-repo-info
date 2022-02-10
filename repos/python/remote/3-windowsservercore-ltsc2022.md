## `python:3-windowsservercore-ltsc2022`

```console
$ docker pull python@sha256:17f0d7e23182906ab0f3f0e43347e04ea66fad17a96a74e0480b9072743992db
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.524; amd64

### `python:3-windowsservercore-ltsc2022` - windows version 10.0.20348.524; amd64

```console
$ docker pull python@sha256:3f7e5127646a07841d07dc865f3336f5d10a43b08de96e82d8f0f84e184b8f52
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2268426631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0f4c53a5da0f648ca52cbbbe33bef481aee7a32efe901ff24646c80c36288db`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Tue, 01 Feb 2022 02:49:40 GMT
RUN Install update ltsc2022-amd64
# Wed, 09 Feb 2022 13:37:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Feb 2022 20:25:10 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 09 Feb 2022 20:31:35 GMT
ENV PYTHON_VERSION=3.10.2
# Wed, 09 Feb 2022 20:32:51 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f ($env:PYTHON_VERSION -replace '[a-z]+[0-9]*$', ''), $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 09 Feb 2022 20:32:53 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 09 Feb 2022 20:32:54 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 09 Feb 2022 20:32:55 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/2caf84b14febcda8077e59e9b8a6ef9a680aa392/public/get-pip.py
# Wed, 09 Feb 2022 20:32:56 GMT
ENV PYTHON_GET_PIP_SHA256=7c5239cea323cadae36083079a5ee6b2b3d56f25762a0c060d2867b89e5e06c5
# Wed, 09 Feb 2022 20:33:40 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 09 Feb 2022 20:33:41 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:898469748ff68223ab87b654b29fb366c1f4f2b7cfad7a37426346ea16db8dfa`  
		Size: 963.2 MB (963225591 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7062696b7aef1ca33afdf32084a532f7e3151a844eb7cb2455bcc907e0f42a58`  
		Last Modified: Wed, 09 Feb 2022 14:28:27 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83e372b4996c8441162dd2ab7b7fc70276cf746df4b5e4d2d8c724b3b69b0099`  
		Last Modified: Wed, 09 Feb 2022 20:44:23 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e41a66f00eba96b62a4c237fe9a6f7a0b2c93bbe7afdc724b7366cc94a7a461`  
		Last Modified: Wed, 09 Feb 2022 20:45:47 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61884a4640bbd000f3c98f226bd37da6c508b798bdbaf408f15009821a522553`  
		Last Modified: Wed, 09 Feb 2022 20:45:54 GMT  
		Size: 46.8 MB (46761599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8440c4bd22e8a6b52ea8f7c0d8a685c45de0c4e125858cb5f541076c2ed3b9f7`  
		Last Modified: Wed, 09 Feb 2022 20:45:47 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d629dfadf0f75ed53504d6bb50683de3f9def2005682fbd23cb0a89a0dff5fe`  
		Last Modified: Wed, 09 Feb 2022 20:45:45 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9dc8e56f28a7eb11242592b21bb099a23a7eafd23efe906d1993ebea30fe614`  
		Last Modified: Wed, 09 Feb 2022 20:45:45 GMT  
		Size: 1.3 KB (1315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46080234a7d2d4aad39b2db4d58aaecd8df854fd4aca0d75fafbd00a645e212b`  
		Last Modified: Wed, 09 Feb 2022 20:45:45 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c36d64cde55c2fe4b57811eb4fed3531b679ba2239beed5040986c0160b19bd`  
		Last Modified: Wed, 09 Feb 2022 20:45:47 GMT  
		Size: 6.7 MB (6729618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579b77891b7cab90b159423819bf12ca14bfbd25c892e7e2fe399aab2f46e2f6`  
		Last Modified: Wed, 09 Feb 2022 20:45:45 GMT  
		Size: 1.3 KB (1320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
