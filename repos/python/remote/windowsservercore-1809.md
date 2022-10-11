## `python:windowsservercore-1809`

```console
$ docker pull python@sha256:cb319f26eb080796beca89d58862e016b0ca1e4c17f909f85dbb89aafb591e3c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `python:windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull python@sha256:6888ced66a6d0c044b6b4bbe8c383efe020bf027b1b47b483b60ca78f5984614
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2764150399 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452c7a88621cef5893819804afb0e07c44b5ac6411208760c52d715fdecfdc60`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 11 Oct 2022 20:24:03 GMT
ENV PYTHONIOENCODING=UTF-8
# Tue, 11 Oct 2022 20:30:27 GMT
ENV PYTHON_VERSION=3.10.7
# Tue, 11 Oct 2022 20:32:21 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f ($env:PYTHON_VERSION -replace '[a-z]+[0-9]*$', ''), $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Tue, 11 Oct 2022 20:32:22 GMT
ENV PYTHON_PIP_VERSION=22.2.2
# Tue, 11 Oct 2022 20:32:23 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Tue, 11 Oct 2022 20:32:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/5eaac1050023df1f5c98b173b248c260023f2278/public/get-pip.py
# Tue, 11 Oct 2022 20:32:25 GMT
ENV PYTHON_GET_PIP_SHA256=5aefe6ade911d997af080b315ebcb7f882212d070465df544e1175ac2be519b4
# Tue, 11 Oct 2022 20:33:50 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$env:PYTHONDONTWRITEBYTECODE = '1'; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Tue, 11 Oct 2022 20:33:51 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:028c482fad0f111537a40f65401f65de54c9fd682951a4f8cf9b644d7c128e18`  
		Size: 834.0 MB (833997855 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c18ec26ea6875d84565b2984f5f26f7abd88d10c281031cda0e675998425247`  
		Last Modified: Tue, 11 Oct 2022 20:35:03 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b20b40a4678efa58eeb4bdf3238faaa46307f136f5a2a58d7b0f26118ee88cc`  
		Last Modified: Tue, 11 Oct 2022 20:35:47 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a7c247a4c850af57c75a33cb2df20e41ef1fa5ad6ce644a2abfd4c0fc6ad8f`  
		Last Modified: Tue, 11 Oct 2022 20:35:53 GMT  
		Size: 49.3 MB (49313888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe12c7cd9f10a0b024594d0489448a463129093dc8f5b184ecef89b6a4b2eec`  
		Last Modified: Tue, 11 Oct 2022 20:35:47 GMT  
		Size: 1.4 KB (1363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26353093f4abd48720473edd18f04602b3aec7ff9548a9edd46942187b8883b`  
		Last Modified: Tue, 11 Oct 2022 20:35:44 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27153e7d3d67e2acd1a523d30a6536077fc891993fb4b261ad2333bd1102bda6`  
		Last Modified: Tue, 11 Oct 2022 20:35:45 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d560cabfe017966357425b0532e55595f3ac2f6cbb62fb6478566b0576a7e50`  
		Last Modified: Tue, 11 Oct 2022 20:35:44 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb3cd489d999317d0f6d35e8ee3918410fc582a8137cac6e1d6b7733359b406`  
		Last Modified: Tue, 11 Oct 2022 20:35:46 GMT  
		Size: 3.7 MB (3661298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9001b27ad1ea896c264f00dada7de3cf07bb6d489279c6aa4a4c3822f1024687`  
		Last Modified: Tue, 11 Oct 2022 20:35:44 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
