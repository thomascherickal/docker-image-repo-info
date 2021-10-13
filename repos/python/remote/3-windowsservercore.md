## `python:3-windowsservercore`

```console
$ docker pull python@sha256:c3b3c017e688cee669ea1a3c0d69d3ddddca8f6d6416808d6a97013e8f3475de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	windows version 10.0.20348.288; amd64
	-	windows version 10.0.17763.2237; amd64
	-	windows version 10.0.14393.4704; amd64

### `python:3-windowsservercore` - windows version 10.0.20348.288; amd64

```console
$ docker pull python@sha256:0e7f850929829cc5a4641dc046e70cead618e083e9ce0ad5ce80eb0acde44b61
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2195440534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:792fc41f1d775893cd6b737d6d2a9ec374e0924238ae20665b0ac622f5a941b1`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 07 Oct 2021 11:33:56 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Oct 2021 12:26:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Oct 2021 17:26:56 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 13 Oct 2021 17:34:07 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 13 Oct 2021 17:34:08 GMT
ENV PYTHON_RELEASE=3.10.0
# Wed, 13 Oct 2021 17:35:40 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 13 Oct 2021 17:35:41 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 13 Oct 2021 17:35:42 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 13 Oct 2021 17:35:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Wed, 13 Oct 2021 17:35:45 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Wed, 13 Oct 2021 17:36:41 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 13 Oct 2021 17:36:42 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b03bbc71f9254a4ad2fba472595c859655b9d0cfefa638928416e277e0f0d497`  
		Size: 889.8 MB (889767519 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b201e45e5b11128e36517715f5b6ae98e5782737c1b112a5fae2aa83206f57bf`  
		Last Modified: Wed, 13 Oct 2021 13:23:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98123f2c4ddfb33c96ba4a6bd915d08c855a3c8a662f0f5b6e166f2c7eb79bc`  
		Last Modified: Wed, 13 Oct 2021 17:57:32 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c80a20136695c56aa18eee8def72045d8098489264d68337d144bde31550e5`  
		Last Modified: Wed, 13 Oct 2021 17:58:13 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d542ca50c9cebf987170089120d7709f0a868a8d6bda8225a2e547693486c70`  
		Last Modified: Wed, 13 Oct 2021 17:58:12 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d38c807ba83039bf6c4fcf7caed86c78afe806244efb558faad3d45660cc5a`  
		Last Modified: Wed, 13 Oct 2021 17:59:05 GMT  
		Size: 47.3 MB (47259063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f50a0470721cb491beb4b8019a0a4381cfdf8e618b8017f2e6c478a56487aaa`  
		Last Modified: Wed, 13 Oct 2021 17:58:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc997eb3054b13080196cdb0f82b2483ba32710b604acd43452dd6b43a9588f`  
		Last Modified: Wed, 13 Oct 2021 17:58:10 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:632aad4ff49e422c4d8d63983348076165c9cf766dc8ea2887f2f2d6fa0795b7`  
		Last Modified: Wed, 13 Oct 2021 17:58:10 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defa69aa67dfdd6c8825394419817956c040aaa56ee18fb30f71b53c642c4100`  
		Last Modified: Wed, 13 Oct 2021 17:58:11 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef6054a81e49b006cf2179294e573220ed5578a3326c15945b697a0f7909ea7`  
		Last Modified: Wed, 13 Oct 2021 17:58:18 GMT  
		Size: 6.7 MB (6702225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0849a3b36bdd7ac7c73cd6f3059df634a56a9bedb67f8a0425fdc0329eadd4a7`  
		Last Modified: Wed, 13 Oct 2021 17:58:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-windowsservercore` - windows version 10.0.17763.2237; amd64

```console
$ docker pull python@sha256:ddcdb5826427b7b81132aa5ee8f51843ce1b1044bac56c992b0def242f9c2b86
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2739814248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca798dbb0d236582031d779a8d8445535391be6203f3e8db52fa6891d3780577`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 07 Oct 2021 08:25:51 GMT
RUN Install update 1809-amd64
# Wed, 13 Oct 2021 12:02:56 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Oct 2021 12:10:58 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 13 Oct 2021 17:36:50 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 13 Oct 2021 17:36:51 GMT
ENV PYTHON_RELEASE=3.10.0
# Wed, 13 Oct 2021 17:39:02 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 13 Oct 2021 17:39:04 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 13 Oct 2021 17:39:05 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 13 Oct 2021 17:39:06 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Wed, 13 Oct 2021 17:39:07 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Wed, 13 Oct 2021 17:40:46 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 13 Oct 2021 17:40:47 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c0698cf91ebd6bcfb319be6a50421b356d6a3dbbd213d9b2b9dca0f837d7a999`  
		Size: 968.0 MB (967985917 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cc0c4e719f418d49c6a0fb87abd2e0e480c5b6fec1bacc3077cacfad9b4ab3e0`  
		Last Modified: Wed, 13 Oct 2021 12:18:09 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a84f5574c99757e575e3da8a06aa95c28164a7daba824decb300ef13da593fb7`  
		Last Modified: Wed, 13 Oct 2021 12:18:44 GMT  
		Size: 1.3 KB (1311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbee6455fddd76d74ecc52a4f9f4dd0b21f15960fbfa96670a55876c749c349`  
		Last Modified: Wed, 13 Oct 2021 17:59:25 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc88ab19f79f5170ee8aa20a08ef7440dff7b49c2861189bffb89852beec842`  
		Last Modified: Wed, 13 Oct 2021 17:59:23 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc051f735ec289820ce5cd714ab4638839a878aaf7a92c00397dd1a60bb63eac`  
		Last Modified: Wed, 13 Oct 2021 18:00:15 GMT  
		Size: 47.0 MB (47022046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e614b8fb30ece62d5a3745f773e3c5b6e954b657c155434b4ff05685acc0913`  
		Last Modified: Wed, 13 Oct 2021 17:59:23 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e8f5966d59b58fe6d4aee5fc7dd9d3648a36140314290e2f540db90827b32b5`  
		Last Modified: Wed, 13 Oct 2021 17:59:21 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d768091a73db0a76337dac99a754ea46db4fd4a875cbec71492dfa06754fb6e`  
		Last Modified: Wed, 13 Oct 2021 17:59:21 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ecbe22ab54f88ba333d0c934af8c57c1dd34681f06f1135f02742e29085c68`  
		Last Modified: Wed, 13 Oct 2021 17:59:25 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2d687373675a6e9fcc138d396da6614bc670c50672c72c96084f66dafaedc4`  
		Last Modified: Wed, 13 Oct 2021 17:59:28 GMT  
		Size: 6.5 MB (6460699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31475f142772c1a04875a254db8ec9458d03a156c24173fb3275370f1274fdc4`  
		Last Modified: Wed, 13 Oct 2021 17:59:21 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `python:3-windowsservercore` - windows version 10.0.14393.4704; amd64

```console
$ docker pull python@sha256:52b7ca29b4a6b9cada82c4b10c752a6a758898b6afabb6f9b885006f341c8182
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6330723313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a545a114bd9cb658785d1e2eb8e1b76d49856141db693ed4369e4245521d6177`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 06 Oct 2021 21:16:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Oct 2021 12:40:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Oct 2021 17:41:04 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 13 Oct 2021 17:41:05 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 13 Oct 2021 17:41:06 GMT
ENV PYTHON_RELEASE=3.10.0
# Wed, 13 Oct 2021 17:43:20 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 13 Oct 2021 17:43:22 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 13 Oct 2021 17:43:23 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 13 Oct 2021 17:43:24 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Wed, 13 Oct 2021 17:43:25 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Wed, 13 Oct 2021 17:45:18 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 13 Oct 2021 17:45:19 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0c776a8e8e3c02d360995b7fa26a3fd7c0928965795fac57b69ff07418ab07bf`  
		Size: 2.2 GB (2202780626 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6974b1bd85ba3f9ce16d86231eced43f720fed9c13411d37584dfe7193bcde60`  
		Last Modified: Wed, 13 Oct 2021 13:27:57 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3055c2d7cf2c2be88d289dc3ae3bf805ce85e1f7024af719a8184af8b0ffe70`  
		Last Modified: Wed, 13 Oct 2021 18:00:35 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03b709cee06fdbba5726e30fa290ec73b8e0d7bef503af5c22cd0bbc76d9ef75`  
		Last Modified: Wed, 13 Oct 2021 18:00:33 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3857450ad45996f3e27ad8b8a773691cba483c32868f76de810e9186f55fd4`  
		Last Modified: Wed, 13 Oct 2021 18:00:33 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7baf280a44d7e63453f2331c08e1791ef390cdd1b4b84b33ccf71b313387bd7c`  
		Last Modified: Wed, 13 Oct 2021 18:01:30 GMT  
		Size: 51.5 MB (51480641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47b100dcb5481e7f3d82e4375e8c0cc84e69f17d7be6bc6e8478329c2e6b4ef`  
		Last Modified: Wed, 13 Oct 2021 18:00:33 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af2bdb6d83bb46ab0da6fa29504b9a6240f09349023ded737012ebcf0ddc162`  
		Last Modified: Wed, 13 Oct 2021 18:00:30 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e72e0947c8b81e326a0cf50bde02eafe65d9514563866a228f178ea0087e0c6`  
		Last Modified: Wed, 13 Oct 2021 18:00:30 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff8ba18614d1720ce74f3d77dfdfc60445362a443e5da5a90fa91b5b5dbc2658`  
		Last Modified: Wed, 13 Oct 2021 18:00:30 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c22d7f0acf0f861bb934f2db666d8ea54ed53217014a1a5f3de25821bc616f68`  
		Last Modified: Wed, 13 Oct 2021 18:00:37 GMT  
		Size: 6.5 MB (6463470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37b16657df9d65878af2dd0d45e29db38a7b5d996e7ae5c2f76e9d55068b2b40`  
		Last Modified: Wed, 13 Oct 2021 18:00:30 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
