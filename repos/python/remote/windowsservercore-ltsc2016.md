## `python:windowsservercore-ltsc2016`

```console
$ docker pull python@sha256:6f848c8a06212873b8e335a21629c533d8a562efc2339265dfa9dfe74936fb52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4651; amd64

### `python:windowsservercore-ltsc2016` - windows version 10.0.14393.4651; amd64

```console
$ docker pull python@sha256:755b553a07b8c685169aa4228740f12549285987aba7d5e08f436bd21beca0bf
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6327522540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9df30fa06c59964a6c33820f81a64257b3490dbcd402a6f109d148a2138dfa46`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 00:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Sep 2021 15:52:22 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 15 Sep 2021 16:00:53 GMT
ENV PYTHON_VERSION=3.9.7
# Wed, 15 Sep 2021 16:00:54 GMT
ENV PYTHON_RELEASE=3.9.7
# Wed, 15 Sep 2021 16:02:30 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 15 Sep 2021 16:02:31 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 15 Sep 2021 16:02:32 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 15 Sep 2021 16:02:33 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Wed, 15 Sep 2021 16:02:34 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Wed, 15 Sep 2021 16:03:52 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 15 Sep 2021 16:03:53 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8721f004192f15fe71b8626ef3f3e34cbf2cfe1d15a63b6b544ab946162ef707`  
		Last Modified: Wed, 15 Sep 2021 01:10:18 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c42d6033c8d973ac20a4c4c23a67c85665485aac081bc572d7778e70fcd0e3bd`  
		Last Modified: Wed, 15 Sep 2021 16:06:16 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1ba49bf1d93737a3cfdaea27cd97134f77df1676dae72530545fa14220e65b`  
		Last Modified: Wed, 15 Sep 2021 16:08:15 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d9564ba6c5256d8db4e6f7c316d4dd174a60c8aa91628817e13b2513f6437a`  
		Last Modified: Wed, 15 Sep 2021 16:08:15 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916c5dd86c573d656447ec834ff91312a82bead5508f6702cdcc6c3fd4df82e3`  
		Last Modified: Wed, 15 Sep 2021 16:09:10 GMT  
		Size: 49.9 MB (49913540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7da8b143904a451242dc66d934533a277fcc058ab3fa4dba00f773ef75ea57`  
		Last Modified: Wed, 15 Sep 2021 16:08:15 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbbcefa43422235514aff083d261ff9c500f9dd2d67f3277886753930f5ade9f`  
		Last Modified: Wed, 15 Sep 2021 16:08:12 GMT  
		Size: 1.3 KB (1308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08615bfcbe77896257061208e5a8eb311d7b1967e6920728633ae0842029f6a8`  
		Last Modified: Wed, 15 Sep 2021 16:08:12 GMT  
		Size: 1.3 KB (1344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34265510b17359cecd63978abbb4df58e484bb00847a7ddcd3c53ad1640b6406`  
		Last Modified: Wed, 15 Sep 2021 16:08:12 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209a21b929077ccc02e074445093859e598d5a70e89fe1246a73b14c098aff6c`  
		Last Modified: Wed, 15 Sep 2021 16:08:14 GMT  
		Size: 6.3 MB (6268896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d8db849f6a7978a9e1d16d604b048b4e00fe8990c13377b8474c4f3e80cdf1`  
		Last Modified: Wed, 15 Sep 2021 16:08:12 GMT  
		Size: 1.3 KB (1302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
