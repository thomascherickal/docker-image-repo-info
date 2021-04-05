## `python:windowsservercore-1809`

```console
$ docker pull python@sha256:476da96472e40146567b5b574b1f0b43285ac727182a26c7686302d85ca1f3b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1817; amd64

### `python:windowsservercore-1809` - windows version 10.0.17763.1817; amd64

```console
$ docker pull python@sha256:bc8cc1a6c793f11c6950e134310cd510daf5bc2f68a85bdf9193b1d75955943a
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2530493625 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5842a0c365310fd5b296b04d5934b01fc3fc4de7e8258b0dd6c5b64e53a935fc`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 27 Feb 2021 09:32:06 GMT
RUN Install update 1809-amd64
# Wed, 10 Mar 2021 13:08:20 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 13:15:52 GMT
ENV PYTHONIOENCODING=UTF-8
# Mon, 05 Apr 2021 17:23:39 GMT
ENV PYTHON_VERSION=3.9.4
# Mon, 05 Apr 2021 17:23:40 GMT
ENV PYTHON_RELEASE=3.9.4
# Mon, 05 Apr 2021 17:25:25 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Mon, 05 Apr 2021 17:25:26 GMT
ENV PYTHON_PIP_VERSION=21.0.1
# Mon, 05 Apr 2021 17:25:27 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/29f37dbe6b3842ccd52d61816a3044173962ebeb/public/get-pip.py
# Mon, 05 Apr 2021 17:25:28 GMT
ENV PYTHON_GET_PIP_SHA256=e03eb8a33d3b441ff484c56a436ff10680479d4bd14e59268e67977ed40904de
# Mon, 05 Apr 2021 17:26:28 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Mon, 05 Apr 2021 17:26:30 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ff1512f88ecd4ff0a91ade34d43733c48834433e35f062f80e6e70d706f8d73`  
		Size: 743.2 MB (743201590 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ebe61daec6d671bc2c1c6fe61ac9825fb552e9cef3672d0a7dbec719d125ae64`  
		Last Modified: Wed, 10 Mar 2021 13:21:09 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f065958960304cba475fb20d779c909f51b0fd4cd8898b3b32e3a57ff66a4170`  
		Last Modified: Wed, 10 Mar 2021 13:23:23 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7cdf4a8c5883217efa3c4b4c139b8e232de794c3bb60f71115a1c00b13de464`  
		Last Modified: Mon, 05 Apr 2021 17:41:49 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060b4bd1732403f425f028fbea846ecfe0bb2ff724ffe9317d17f6641e6aab9a`  
		Last Modified: Mon, 05 Apr 2021 17:41:49 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6d6a2b6d7135c6f0d96852875818483a669eb0e4508343b9ef0439b4ffe04f`  
		Last Modified: Mon, 05 Apr 2021 17:42:59 GMT  
		Size: 58.6 MB (58646130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9855750e77119a147f02e9029cc0a68bf5c7836f4fd7b71b140d0f74d38e5789`  
		Last Modified: Mon, 05 Apr 2021 17:41:47 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e352d4d75cc5ad698cea5c1b47718f50c81d4d3e179f39a78059b87a5b9c2742`  
		Last Modified: Mon, 05 Apr 2021 17:41:47 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d115f06854bb89d7fc4cdfda7a1693fcc789c1b8109198e27683db879e75e20`  
		Last Modified: Mon, 05 Apr 2021 17:41:47 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f161a00a20339acddb41a80a9a1c172de3a8f4b1242ca8dfd5ba155d41937a`  
		Last Modified: Mon, 05 Apr 2021 17:41:50 GMT  
		Size: 10.3 MB (10301632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84766a84248f60b84f529bcc865ca2450e3c89715b8ca3dff85bab0e7cf04366`  
		Last Modified: Mon, 05 Apr 2021 17:41:47 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
