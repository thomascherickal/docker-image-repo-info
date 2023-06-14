## `python:windowsservercore-ltsc2022`

```console
$ docker pull python@sha256:0a58f0ab5ab41ceec6a3a692f927ec2b4691478d29fb13b8364309eba32efec9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1787; amd64

### `python:windowsservercore-ltsc2022` - windows version 10.0.20348.1787; amd64

```console
$ docker pull python@sha256:eaf4991f7c1256f64a6840aff43ccc6dda136eff36041bab133ebd81fc1b67dc
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1444857237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78b6aa8f665d37c3ba2f926525e7a492dad952b0ee30f847edf96120c17957ab`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 08 Jun 2023 12:55:20 GMT
RUN Apply image 10.0.20348.1787
# Wed, 14 Jun 2023 17:38:14 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Jun 2023 23:00:57 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 14 Jun 2023 23:12:12 GMT
ENV PYTHON_VERSION=3.11.4
# Wed, 14 Jun 2023 23:13:27 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f ($env:PYTHON_VERSION -replace '[a-z]+[0-9]*$', ''), $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 14 Jun 2023 23:13:28 GMT
ENV PYTHON_PIP_VERSION=23.1.2
# Wed, 14 Jun 2023 23:13:29 GMT
ENV PYTHON_SETUPTOOLS_VERSION=65.5.1
# Wed, 14 Jun 2023 23:13:30 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/0d8570dc44796f4369b652222cf176b3db6ac70e/public/get-pip.py
# Wed, 14 Jun 2023 23:13:31 GMT
ENV PYTHON_GET_PIP_SHA256=96461deced5c2a487ddc65207ec5a9cffeca0d34e7af7ea1afc470ff0d746207
# Wed, 14 Jun 2023 23:14:16 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$env:PYTHONDONTWRITEBYTECODE = '1'; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 14 Jun 2023 23:14:16 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:7c76e5cf7755ce357ffb737715b0da6799a50ea468cc252c094f4d915d426b3f`  
		Last Modified: Tue, 13 Jun 2023 17:55:32 GMT  
		Size: 1.4 GB (1388598786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0972ddd233121a2afd2cf1a3eaec49d595cfe6b3ebe19ef3dd492d99784c370f`  
		Last Modified: Wed, 14 Jun 2023 18:17:55 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d609ded9dc6380f940e099871299c633bd50eb969deeeb317866a4f36a86d253`  
		Last Modified: Wed, 14 Jun 2023 23:17:34 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e900be69bea6f73d01ca445551d3835801cacd40624d3e31f22255beed560e7a`  
		Last Modified: Wed, 14 Jun 2023 23:18:10 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39843cce3ec5ec9938f217e7008c16ca1f88e7b78b1958bb3421c4bc2398b04`  
		Last Modified: Wed, 14 Jun 2023 23:18:17 GMT  
		Size: 50.6 MB (50599403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c967c7c16dcc3ae9d947614d9ff781f6949bc174dc93fe22506dabbef2076342`  
		Last Modified: Wed, 14 Jun 2023 23:18:10 GMT  
		Size: 1.3 KB (1323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cea209e44514e1c7108c0bab5dce5e8b378ab90a1f68bba80e38e9a20cdc973`  
		Last Modified: Wed, 14 Jun 2023 23:18:08 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d48ea6b27083264593b46ddf951748bd190ec7465553baa1f2577be40884523c`  
		Last Modified: Wed, 14 Jun 2023 23:18:08 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:820515414e8b50aadb06538efa456382f3fc1085b2ffc084fb48f6971ac33c4b`  
		Last Modified: Wed, 14 Jun 2023 23:18:08 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f1e7f494e3343fd9082c48cf22ef803046326cd51cac26c2b5df6b06401e3fe`  
		Last Modified: Wed, 14 Jun 2023 23:18:10 GMT  
		Size: 5.6 MB (5648592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8924ec8dbbba2a28059f7133c2eef6e321f0780bd350bf9ebfe34b5f09b408`  
		Last Modified: Wed, 14 Jun 2023 23:18:08 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
