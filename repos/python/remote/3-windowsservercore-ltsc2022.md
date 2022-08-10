## `python:3-windowsservercore-ltsc2022`

```console
$ docker pull python@sha256:8ea5767f169954fd2ef2d4abc04c0de3b40cbb4854c4d7b9f608a1c0fe816c23
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.887; amd64

### `python:3-windowsservercore-ltsc2022` - windows version 10.0.20348.887; amd64

```console
$ docker pull python@sha256:efa5e2771413006c2617140a8d704ac01a7df79a13b5539e8f9fc4bc95c8e76f
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2370375114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eceb5e0e425f2d88a3dee237f333b1f2a54e3b573aa6442c1f79d62b3401181c`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 12:11:45 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 12:33:23 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 10 Aug 2022 15:37:43 GMT
ENV PYTHON_VERSION=3.10.6
# Wed, 10 Aug 2022 15:38:54 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f ($env:PYTHON_VERSION -replace '[a-z]+[0-9]*$', ''), $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 15:38:55 GMT
ENV PYTHON_PIP_VERSION=22.2.1
# Wed, 10 Aug 2022 15:38:56 GMT
ENV PYTHON_SETUPTOOLS_VERSION=63.2.0
# Wed, 10 Aug 2022 15:38:57 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/aeca83c7ba7f9cdfd681103c4dcbf0214f6d742e/public/get-pip.py
# Wed, 10 Aug 2022 15:38:58 GMT
ENV PYTHON_GET_PIP_SHA256=d0b5909f3ab32dae9d115aa68a4b763529823ad5589c56af15cf816fca2773d6
# Wed, 10 Aug 2022 15:39:39 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$env:PYTHONDONTWRITEBYTECODE = '1'; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 10 Aug 2022 15:39:40 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4a5e3787c778295a5877e0381020b02273a985f7db2dd483ddff586869546e4c`  
		Last Modified: Wed, 10 Aug 2022 12:42:34 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8259ecb0e5034b8fa5de016424036c94452d1ef91533fce60f0ac1e95aa4e543`  
		Last Modified: Wed, 10 Aug 2022 12:45:16 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dede03b6cf0aec7439df57efcd398f9967add637f94e63eb43e1e9e1e2323a60`  
		Last Modified: Wed, 10 Aug 2022 15:50:24 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ccdf04430f2c9ba909e3ecc8a520ae02e9d36fb78de306993068ce59dd6b4c`  
		Last Modified: Wed, 10 Aug 2022 15:50:31 GMT  
		Size: 49.6 MB (49553247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93185a5fc9a930e59aaf22153314017bf82bb0a51e77c2b590a5592969b48f1`  
		Last Modified: Wed, 10 Aug 2022 15:50:23 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:998b0703e53d54c77a5305ff44350e53c43c6bd9d99605bd32bd1b4cc4de54cd`  
		Last Modified: Wed, 10 Aug 2022 15:50:21 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35779712110d4405bb93dccc5de48e49e49d794bb07bc41252f671585bbf80af`  
		Last Modified: Wed, 10 Aug 2022 15:50:21 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e78c952fa0e54f90ee01e2821de6c3bc83bc04e48c3f2ffd66693b45ec4bb3c`  
		Last Modified: Wed, 10 Aug 2022 15:50:21 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257ea0c7ae895fb8a94e26122451aecda96eae1767dd5f434e8e93423c08e294`  
		Last Modified: Wed, 10 Aug 2022 15:50:23 GMT  
		Size: 3.9 MB (3921463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45691e76de5dcdd2be781006ad1c5f78e1779742403a687074dcbd6073827ea4`  
		Last Modified: Wed, 10 Aug 2022 15:50:22 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
