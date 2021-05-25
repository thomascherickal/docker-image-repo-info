## `hylang:python3.8-windowsservercore-1809`

```console
$ docker pull hylang@sha256:886a432e826e50d523693f97e3002bab7ec5176aeda19cb5df1e56384dafe522
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `hylang:python3.8-windowsservercore-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull hylang@sha256:8df795d109606a0ee93e9f1b2698b2392f7738d621647679011925c623d4dd80
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2535762018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ce96921a68705e15f11707e30284f6b45d295ce63607743c61c342f873f6d86`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 08 May 2021 09:21:48 GMT
RUN Install update 1809-amd64
# Wed, 12 May 2021 12:10:17 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 12:15:16 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 12 May 2021 16:06:33 GMT
ENV PYTHON_VERSION=3.8.10
# Wed, 12 May 2021 16:06:35 GMT
ENV PYTHON_RELEASE=3.8.10
# Wed, 12 May 2021 16:08:28 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Mon, 24 May 2021 19:22:35 GMT
ENV PYTHON_PIP_VERSION=21.1.2
# Mon, 24 May 2021 19:22:36 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/936e08ce004d0b2fae8952c50f7ccce1bc578ce5/public/get-pip.py
# Mon, 24 May 2021 19:22:36 GMT
ENV PYTHON_GET_PIP_SHA256=8890955d56a8262348470a76dc432825f61a84a54e2985a86cd520f656a6e220
# Mon, 24 May 2021 19:23:31 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Mon, 24 May 2021 19:23:32 GMT
CMD ["python"]
# Mon, 24 May 2021 19:50:03 GMT
ENV HY_VERSION=1.0a1
# Mon, 24 May 2021 19:50:40 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Mon, 24 May 2021 19:50:41 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8116de3c91c3f1ef2d6c09b49ef5407c9b4d672896eb3af5182a997c3c5379c9`  
		Size: 756.2 MB (756156286 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5b8861e3624ab787e21ee36b876b374a3b5ec40eed1621cebfe2f81d1c2cda37`  
		Last Modified: Wed, 12 May 2021 12:20:32 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9aa1c8ec0c5a4f42cff7e6de598f0e6cc847b6806a9261b7989f4a96fdbd1f`  
		Last Modified: Wed, 12 May 2021 12:21:24 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecab1eeb7d320c5061b2d9dfb53a18e6fea50c9b3328cd2bd8fb67319a919463`  
		Last Modified: Wed, 12 May 2021 16:17:47 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2864792a173d9828ba7d573aa616e02e62f4a1666b41d7d677d4d25f75c41cfc`  
		Last Modified: Wed, 12 May 2021 16:17:47 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028af68cf3ec3a5ef87a754a6d2d8b579295cbc7a4ca9dd15ba47369719054dd`  
		Last Modified: Wed, 12 May 2021 16:17:57 GMT  
		Size: 53.8 MB (53783029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fd123c72cc41802064bcda6c4d2c4428ce044438cfafc95bdd9f6b99971c4f`  
		Last Modified: Mon, 24 May 2021 19:28:13 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9876f1cef2b734debf35737ea8b8101b99976cb738b2a70495022b47148a4629`  
		Last Modified: Mon, 24 May 2021 19:28:14 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf530d6f0ca7470a934a31c7d748cc17b9693b1942700090188bd5961ff1a4de`  
		Last Modified: Mon, 24 May 2021 19:28:13 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d8e2c5d67e21b8583bd338330bd38d6d0c033f9ce80743448e8f9d80ed0c07`  
		Last Modified: Mon, 24 May 2021 19:28:15 GMT  
		Size: 6.3 MB (6268275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f526af53841ff2ef15004f803fc335e33e0c00cf86e01a86d530f8ffd0b7bc2b`  
		Last Modified: Mon, 24 May 2021 19:28:13 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:710fab1cd1c6e2760b49dc19878bd47710ca2a9a6fac2daf7613c3e909df4064`  
		Last Modified: Mon, 24 May 2021 19:58:15 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8505faad1fc71fc6f3a0cbbaeb7b3a3f002e613978673b6adc5d2f0f5f20aadc`  
		Last Modified: Mon, 24 May 2021 19:58:16 GMT  
		Size: 1.2 MB (1207366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39f2a5e207558ec13902a814f50e3267481166f2b2c24092fc5c9ae2f4ba2d0`  
		Last Modified: Mon, 24 May 2021 19:58:15 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
