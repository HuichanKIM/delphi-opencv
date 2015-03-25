# Delphi-OpenCV #

OpenCV version - 2.4.9<br>
Development environment - Delphi 2010-XE7<br>
<br>
Requires installed <a href='http://www.microsoft.com/ru-ru/download/details.aspx?id=40784'>Visual C++ redistributable for Visual Studio 2013</a>

<h3>Contributors:</h3>
<pre><code> Laentir Valetov (email: laex@bk.ru)<br>
 Mikhail Grigorev (email: sleuthhound@gmail.com)<br>
</code></pre>
<h2>How to install:</h2>
Download the <a href='https://github.com/Laex/Delphi-OpenCV/archive/master.zip'>archive</a>
Unzip it to a convenient directory, thus get the following directory structure<br>
<pre><code>PROJECT_ROOT&gt; - Directory, such as "C:\OpenCV\"<br>
	&lt;bin&gt;<br>
	&lt;redist&gt;<br>
	&lt;resource&gt;<br>
	&lt;samples&gt;<br>
	&lt;source&gt;<br>
</code></pre>
Add the search path for the modules of the project in Delphi IDE (Tools-Options-Delphi Options-Library-Library path)<br>
<pre><code>&lt;PROJECT_ROOT&gt;\source<br>
&lt;PROJECT_ROOT&gt;\source\utils<br>
&lt;PROJECT_ROOT&gt;\source\component<br>
&lt;PROJECT_ROOT&gt;\source\sdl<br>
&lt;PROJECT_ROOT&gt;\source\opengl<br>
&lt;PROJECT_ROOT&gt;\source\ffmpeg<br>
&lt;PROJECT_ROOT&gt;\resource\facedetectxml<br>
</code></pre>
where <code>&lt;PROJECT_ROOT&gt;</code> directory, which was unzipped project.<br>
Add to your PATH variable path to the library "opencv<b><b>.dll" and FFMPEG dll.<br></b> for Win32 <code>&lt;PROJECT_ROOT&gt;\bin\Win32</code>
<i>for Win64 <code>&lt;PROJECT_ROOT&gt;\bin\Win64</code></i>

Or</b>

For 64-bit<br>
<pre><code>1. Copy the dll files from the &lt;PROJECT_ROOT&gt;\redist\VC2013x64\ to C:\Windows\System32\<br>
2. Copy all the dll from &lt;PROJECT_ROOT&gt;\bin\Win64 in the C:\Windows\System32\<br>
3. Copy the dll files from the &lt;PROJECT_ROOT&gt;\redist\VC2013x86\ to C:\Windows\SysWOW64\<br>
4. Copy all the dll from &lt;PROJECT_ROOT&gt;\bin\Win32 in the C:\Windows\SysWOW64\<br>
</code></pre>
For 32-bit<br>
<pre><code>1. Copy the dll files from the &lt;PROJECT_ROOT&gt;\redist\VC2013x86\ to C:\Windows\System32\<br>
2. Copy all the dll from &lt;PROJECT_ROOT&gt;\bin\Win32 in the C:\Windows\System32\<br>
</code></pre>
To install the components, open and install<br>
<pre><code>&lt;PROJECT_ROOT&gt;\source\component\DelphiXX\OpenCVXXX.dpk<br>
&lt;PROJECT_ROOT&gt;\source\component\DelphiXX\dclCommonOpenCVXXX.dpk<br>
&lt;PROJECT_ROOT&gt;\source\component\DelphiXX\dclVCLOpenCVXXX.dpk<br>
&lt;PROJECT_ROOT&gt;\source\component\DelphiXX\dclFMXOpenCVXXX.dpk<br>
</code></pre>
Open in Delphi IDE and compile:<br>
Examples of the use of certain functions and procedures<br>
<pre><code>&lt;PROJECT_ROOT&gt;\samples\LibDemo\LibDemo.groupproj<br>
</code></pre>
Examples of the use of video processing algorithms<br>
<pre><code>&lt;PROJECT_ROOT&gt;\samples\MultiDemo\MultiDemo.groupproj<br>
</code></pre>
Examples of the use of video processing algorithms using VCL.Forms<br>
<pre><code>&lt;PROJECT_ROOT&gt;\samples\VCLDemo\VCLDemo.groupproj<br>
</code></pre>
Examples of using FFMPEG library header files are in the<br>
<pre><code>&lt;PROJECT_ROOT&gt;\samples\FFMpeg\FFMPEG.groupproj<br>
</code></pre>
Examples of use of components<br>
<pre><code>&lt;PROJECT_ROOT&gt;\samples\Components\ComponentsDemo.groupproj<br>
</code></pre>