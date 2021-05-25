## `hylang:python3.10-rc-windowsservercore-ltsc2016`

```console
$ docker pull hylang@sha256:68445bef3168b8c2bdcfaa40b86327c5aa3e4b2bdb0e03c202ca8e5a3b79d2c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4402; amd64

### `hylang:python3.10-rc-windowsservercore-ltsc2016` - windows version 10.0.14393.4402; amd64

```console
$ docker pull hylang@sha256:67612bf0245bca1a4a83e3849d1aa19f2e519bb620932e001c2db2da7909d0b3
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5870534463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d868de325921149fd7c0fa00cabd047262a42aaae9eea9dc1ecfebf3756f9c2`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 26 Apr 2021 17:25:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 12 May 2021 12:29:11 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 May 2021 15:53:37 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 12 May 2021 15:53:38 GMT
ENV PYTHON_VERSION=3.10.0b1
# Wed, 12 May 2021 15:53:39 GMT
ENV PYTHON_RELEASE=3.10.0
# Wed, 12 May 2021 15:56:14 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Mon, 24 May 2021 19:16:39 GMT
ENV PYTHON_PIP_VERSION=21.1.2
# Mon, 24 May 2021 19:16:40 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/936e08ce004d0b2fae8952c50f7ccce1bc578ce5/public/get-pip.py
# Mon, 24 May 2021 19:16:42 GMT
ENV PYTHON_GET_PIP_SHA256=8890955d56a8262348470a76dc432825f61a84a54e2985a86cd520f656a6e220
# Mon, 24 May 2021 19:18:52 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Mon, 24 May 2021 19:18:54 GMT
CMD ["python"]
# Mon, 24 May 2021 19:53:31 GMT
ENV HY_VERSION=1.0a1
# Mon, 24 May 2021 19:55:22 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Mon, 24 May 2021 19:55:23 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7f532f88613ca85064b055f6b93f8517bd05feba8fdce495a6ad1421573e765e`  
		Size: 1.7 GB (1725791397 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a280ee47051c0dfafc65e567f555ec59b7415288f965b44cf55c9187407d4248`  
		Last Modified: Wed, 12 May 2021 12:55:16 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f317eeb27434208e414af5c9ea59122edf0255981d63b909521facca8e43ab6`  
		Last Modified: Wed, 12 May 2021 16:16:16 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6db25fec8291c92a3d9fc7ebf8f1a49c18158c24f5f1bf3507e8e16035d8191`  
		Last Modified: Wed, 12 May 2021 16:16:15 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcb7f1fd1609b442a2190d7eb0e53877596edf5d8f52e7c334b404dbdd8391af`  
		Last Modified: Wed, 12 May 2021 16:16:15 GMT  
		Size: 1.4 KB (1371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab06b566b54aeb7a785e5d105f1b882c5a9669cb3fe57a088eaad9f88d30b01`  
		Last Modified: Wed, 12 May 2021 16:16:25 GMT  
		Size: 56.5 MB (56465354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c19ddf3ddf255d28f89b55c1dd78a0e0ccf83d8345bab5311fd50d4da090090e`  
		Last Modified: Mon, 24 May 2021 19:27:13 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a5931950bd085b64e4f63da28264979912fda2a6c980cffbc3178e856674b1`  
		Last Modified: Mon, 24 May 2021 19:27:13 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48ec3f2a6cbb012b2452dab567cf9c23d0b8dc3ac4cd184621bd3c5901921c9e`  
		Last Modified: Mon, 24 May 2021 19:27:13 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ef9bdf30d0f588bc40f4319704a326e193f6bb2af7c35eb190b03eab45353c`  
		Last Modified: Mon, 24 May 2021 19:27:17 GMT  
		Size: 11.8 MB (11778512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b34dc43d37ddb850833eb317f4526870efe5e4530b3370d705aef728fa12127`  
		Last Modified: Mon, 24 May 2021 19:27:13 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75fbf2ae544c94bde3a5ded6972ee532901968444e5a4e69bf35ad9202c2983`  
		Last Modified: Mon, 24 May 2021 19:58:52 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b395f88fe270404d03b179f084c126aad4919f38313a14b0f2a4c55a6eb94f2`  
		Last Modified: Mon, 24 May 2021 19:58:54 GMT  
		Size: 6.5 MB (6499077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c377f89dc81108794e517f01ca2354a1d81695d4175be02b1794c5ff9a5d2c5c`  
		Last Modified: Mon, 24 May 2021 19:58:53 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
