## `pypy:2-windowsservercore-ltsc2022`

```console
$ docker pull pypy@sha256:3f2e6caf5c4f88f01c123a73303440773345d01fd99496886fb2974471f7328b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.587; amd64

### `pypy:2-windowsservercore-ltsc2022` - windows version 10.0.20348.587; amd64

```console
$ docker pull pypy@sha256:f9d352f0f88c1cdda0de96739b3ddbdb3b5401d3ee0ae1ba85c7f3ea1f569eff
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2263116884 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:911d9db87131fe98c6bf633baa9e897bda718e841432461957ea97f50f1f614f`
-	Default Command: `["pypy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 03 Mar 2022 05:02:11 GMT
RUN Install update ltsc2022-amd64
# Tue, 08 Mar 2022 19:26:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Tue, 08 Mar 2022 19:50:28 GMT
ENV PYTHONIOENCODING=UTF-8
# Tue, 08 Mar 2022 19:50:57 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Tue, 08 Mar 2022 19:51:29 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Tue, 08 Mar 2022 19:51:30 GMT
ENV PYPY_VERSION=7.3.8
# Tue, 08 Mar 2022 19:52:24 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy2.7-v7.3.8-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = '806a29a6c5550b1e669d8870683d3379138d3d43eb1e07bdf26d65a0691265f2'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy2.7-v7.3.8-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy --version") ...'; 	pypy --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Tue, 08 Mar 2022 19:52:27 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Tue, 08 Mar 2022 19:52:28 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Tue, 08 Mar 2022 19:53:30 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Tue, 08 Mar 2022 19:53:32 GMT
CMD ["pypy"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:037d5740b40414bc505c21324142a1cd3eab10c176189a9a74d1a90354ac7cd4`  
		Size: 969.5 MB (969547968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d58ba398110c3f761c6307a5621ec218b8593ba8b07b734436bcdd8d07a23e08`  
		Last Modified: Tue, 08 Mar 2022 20:00:31 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2670129d6f6229df67ced77db459e0185e71cc16013f2d92247a4cef3720a1`  
		Last Modified: Tue, 08 Mar 2022 20:04:10 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f139349090948bed54214d9e139d639c91f7d446842a6952af850a3b7007933`  
		Last Modified: Tue, 08 Mar 2022 20:04:09 GMT  
		Size: 598.1 KB (598056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e46dd2d39364df753a76d0f02c866f45bd888bfbb5ff3d7fd624be5b774814b6`  
		Last Modified: Tue, 08 Mar 2022 20:04:11 GMT  
		Size: 15.7 MB (15701008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5185e05c65d139d8f9f773d9e0021f972061725f566106738a1e514a8a70ce`  
		Last Modified: Tue, 08 Mar 2022 20:04:09 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fedaadd59f6c33b0381a79876dbe0dd3f6baa7d56735e7d54577083dc6903bab`  
		Last Modified: Tue, 08 Mar 2022 20:04:33 GMT  
		Size: 22.8 MB (22763690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a55c7b93f71b5ed7e6aea62206b9ea3569615040a5071030f64ba0e083d0b2`  
		Last Modified: Tue, 08 Mar 2022 20:04:06 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f832d903f3ff65297eb5d41cfbcc37436f778f90932e3238b7f24b85d0ea8c`  
		Last Modified: Tue, 08 Mar 2022 20:04:06 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0160cd4a1a8cab06a767c2f9846eab31502beac526c63afdc5429ec6a20c4f9`  
		Last Modified: Tue, 08 Mar 2022 20:04:07 GMT  
		Size: 2.8 MB (2798662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae73ba0636c0312ad65a3bff5dc7aff37753f03f7ea89ae44c3d23370a5d5aa`  
		Last Modified: Tue, 08 Mar 2022 20:04:06 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
