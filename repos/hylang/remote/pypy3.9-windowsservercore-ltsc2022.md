## `hylang:pypy3.9-windowsservercore-ltsc2022`

```console
$ docker pull hylang@sha256:135bea03611d5b1b542c71d62dbaaed3678eaf9b329ee6b8007cf46a3cf40bc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.643; amd64

### `hylang:pypy3.9-windowsservercore-ltsc2022` - windows version 10.0.20348.643; amd64

```console
$ docker pull hylang@sha256:1647b83f38bb24eac602ff1286edc96c5552645a14d3d8ebd6080c5bc35b7373
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2277029550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52567c3f7f240185d4bc4528c4020875e08deabe7f127757d8fceac150ba901e`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 03 Apr 2022 05:50:25 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Apr 2022 02:27:58 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Apr 2022 12:03:22 GMT
RUN $newPath = ('C:\pypy;C:\pypy\Scripts;{0}' -f $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine); 	Write-Host 'Complete.'
# Wed, 13 Apr 2022 12:03:51 GMT
RUN $url = 'https://download.microsoft.com/download/6/A/A/6AA4EDFF-645B-48C5-81CC-ED5963AEAD48/vc_redist.x64.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'vc.exe'; 		$sha256 = 'da66717784c192f1004e856bbcf7b3e13b7bf3ea45932c48e4c9b9a50ca80965'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash vc.exe -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process 		-NoNewWindow 		-Wait 		-FilePath .\vc.exe 		-ArgumentList @( 			'/install', 			'/quiet', 			'/norestart' 		); 		Write-Host 'Removing ...'; 	Remove-Item vc.exe -Force; 		Write-Host 'Complete.'
# Wed, 13 Apr 2022 12:03:52 GMT
ENV PYPY_VERSION=7.3.9
# Wed, 13 Apr 2022 12:04:45 GMT
RUN $url = 'https://downloads.python.org/pypy/pypy3.9-v7.3.9-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'pypy.zip'; 		$sha256 = 'be48ab42f95c402543a7042c999c9433b17e55477c847612c8733a583ca6dff5'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash pypy.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive pypy.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item pypy.zip -Force; 		Write-Host 'Renaming ...'; 	Rename-Item -Path C:\pypy3.9-v7.3.9-win64 -NewName C:\pypy; 		Write-Host 'Verifying install ("pypy --version") ...'; 	pypy --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 13 Apr 2022 12:04:46 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/3843bff3a0a61da5b63ea0b7d34794c5c51a2f11/get-pip.py
# Wed, 13 Apr 2022 12:04:47 GMT
ENV PYTHON_GET_PIP_SHA256=95c5ee602b2f3cc50ae053d716c3c89bea62c58568f64d7d25924d399b2d5218
# Wed, 13 Apr 2022 12:05:59 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$pipVersion = & pypy -c 'import ensurepip; print(ensurepip._PIP_VERSION)'; 	$setuptoolsVersion = & pypy -c 'import ensurepip; print(ensurepip._SETUPTOOLS_VERSION)'; 		Write-Host ('Installing "pip == {0}", "setuptools == {1}" ...' -f $pipVersion, $setuptoolsVersion); 	pypy get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip == {0}' -f $pipVersion) 		('setuptools == {0}' -f $setuptoolsVersion) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Cleanup install ...'; 	Get-ChildItem 		-Path C:\pypy 		-Include @( 'test', 'tests' ) 		-Directory 		-Recurse 		| Remove-Item -Force -Recurse; 	Get-ChildItem 		-Path C:\pypy 		-Include @( '*.pyc', '*.pyo' ) 		-File 		-Recurse 		| Remove-Item -Force; 		Write-Host 'Complete.'
# Wed, 13 Apr 2022 12:06:00 GMT
CMD ["pypy"]
# Wed, 27 Apr 2022 12:29:17 GMT
ENV HY_VERSION=1.0a4
# Wed, 27 Apr 2022 12:29:18 GMT
ENV HYRULE_VERSION=0.1
# Wed, 27 Apr 2022 12:30:17 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Wed, 27 Apr 2022 12:30:18 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dccd9e4d14d3d5a6e93f87350b903e117368ada32d711986f779b5a3ef8657cc`  
		Size: 975.3 MB (975255801 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1ab01d498c34190a1e49e15239442a41312c6ea5904e18f186f84f90f11fc422`  
		Last Modified: Wed, 13 Apr 2022 03:13:51 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96ac23d5eccd67c034cb6932c218fb1737e542524efd6238e082ecdf54ae0ea`  
		Last Modified: Wed, 27 Apr 2022 12:07:12 GMT  
		Size: 627.8 KB (627831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc394bd04379f4961d1bd7dfb6e6b46f9617d3017c8b96a74b98e6166f48441`  
		Last Modified: Wed, 27 Apr 2022 12:07:29 GMT  
		Size: 15.8 MB (15750648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f19529246a74ac80fe7f83fab4502ebf427265a76e628f281889a92fef1373d6`  
		Last Modified: Wed, 27 Apr 2022 12:07:11 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664242fc796b5e799cb1a94bb8ab301f1aa871dc8467f9c7c34d44a5d409e040`  
		Last Modified: Wed, 27 Apr 2022 12:07:20 GMT  
		Size: 26.6 MB (26613051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd1ff9006a9ea33ae176547130a7e118e3d03b762484e56f72ecd7b73fa33564`  
		Last Modified: Wed, 27 Apr 2022 12:07:09 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c741e49247d317c1087baa9b58549e5010916b7235c6ec8e6f4b4ce2fb297b`  
		Last Modified: Wed, 27 Apr 2022 12:07:09 GMT  
		Size: 1.3 KB (1307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f2127453c25f3c6eeb4747f3e0a141f2fc6f01af6dad51005ce3b9d7681a30`  
		Last Modified: Wed, 27 Apr 2022 12:07:13 GMT  
		Size: 3.2 MB (3238959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e24e717dee7a041bbcc7f1315f1a32d1623a0038d8c8f8615d179f70ba990c7`  
		Last Modified: Wed, 27 Apr 2022 12:07:09 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b034c7bdd4e814d2608080fa93e4d0bc11e2f30792d042e63522ea1ee8ce9bda`  
		Last Modified: Wed, 04 May 2022 12:03:14 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f2ddd36bfbc4a5fee16df43d418f597d6fda04e5a4a0d992d579e7d69cda65f`  
		Last Modified: Wed, 04 May 2022 12:03:14 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b2815e107c6e6cea157d19b69b3bfba253bf4d263668d35c19b03c329a647b`  
		Last Modified: Wed, 04 May 2022 12:03:18 GMT  
		Size: 3.8 MB (3833223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79ccd078a7b160d8a9eca91b166bccafd66def8c6fce3bbfcc62d4e3a18338f6`  
		Last Modified: Wed, 04 May 2022 12:03:14 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
