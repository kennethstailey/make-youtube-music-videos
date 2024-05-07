Example invocations:
```
$ ls
input.jpg  input.mp3  make-youtube-music-videos

$ ./make-youtube-music-videos 
Please use three values, a JPEG, an audio in mp3 or flac
and the name of the output file, mp4 is best.

$ ./make-youtube-music-videos input.jpg input.mp3 output.mp4
ffmpeg version n6.1.1 Copyright (c) 2000-2023 the FFmpeg developers
  built with gcc 13.2.1 (GCC) 20230801
  configuration: --prefix=/usr --disable-debug --disable-static --disable-stripping --enable-amf --enable-avisynth --enable-cuda-llvm --enable-lto --enable-fontconfig --enable-frei0r --enable-gmp --enable-gnutls --enable-gpl --enable-ladspa --enable-libaom --enable-libass --enable-libbluray --enable-libbs2b --enable-libdav1d --enable-libdrm --enable-libfreetype --enable-libfribidi --enable-libgsm --enable-libharfbuzz --enable-libiec61883 --enable-libjack --enable-libjxl --enable-libmodplug --enable-libmp3lame --enable-libopencore_amrnb --enable-libopencore_amrwb --enable-libopenjpeg --enable-libopenmpt --enable-libopus --enable-libplacebo --enable-libpulse --enable-librav1e --enable-librsvg --enable-librubberband --enable-libsnappy --enable-libsoxr --enable-libspeex --enable-libsrt --enable-libssh --enable-libsvtav1 --enable-libtheora --enable-libv4l2 --enable-libvidstab --enable-libvmaf --enable-libvorbis --enable-libvpl --enable-libvpx --enable-libwebp --enable-libx264 --enable-libx265 --enable-libxcb --enable-libxml2 --enable-libxvid --enable-libzimg --enable-nvdec --enable-nvenc --enable-opencl --enable-opengl --enable-shared --enable-vapoursynth --enable-version3 --enable-vulkan
  libavutil      58. 29.100 / 58. 29.100
  libavcodec     60. 31.102 / 60. 31.102
  libavformat    60. 16.100 / 60. 16.100
  libavdevice    60.  3.100 / 60.  3.100
  libavfilter     9. 12.100 /  9. 12.100
  libswscale      7.  5.100 /  7.  5.100
  libswresample   4. 12.100 /  4. 12.100
  libpostproc    57.  3.100 / 57.  3.100
Input #0, image2, from 'input.jpg':
  Duration: 00:00:00.04, start: 0.000000, bitrate: 33905 kb/s
  Stream #0:0: Video: mjpeg (Baseline), yuvj444p(pc, bt470bg/unknown/unknown), 596x599, 25 fps, 25 tbr, 25 tbn
Input #1, mp3, from 'input.mp3':
  Metadata:
    title           : genius
    artist          : lispector
    album           : human problems and how to solv
    date            : 2002
    comment         : julie rox!
    genre           : Pop-Folk
  Duration: 00:04:58.37, start: 0.025057, bitrate: 136 kb/s
  Stream #1:0: Audio: mp3, 44100 Hz, stereo, fltp, 136 kb/s
    Metadata:
      encoder         : LAME3.92 
Stream mapping:
  Stream #0:0 -> #0:0 (mjpeg (native) -> h264 (libx264))
  Stream #1:0 -> #0:1 (mp3 (mp3float) -> aac (native))
Press [q] to stop, [?] for help
[libx264 @ 0x64f136c7eb80] using cpu capabilities: MMX2 SSE2Fast SSSE3 SSE4.2 AVX FMA3 BMI2 AVX2
[libx264 @ 0x64f136c7eb80] profile High 4:4:4 Predictive, level 2.2, 4:4:4, 8-bit
[libx264 @ 0x64f136c7eb80] 264 - core 164 r3108 31e19f9 - H.264/MPEG-4 AVC codec - Copyleft 2003-2023 - http://www.videolan.org/x264.html - options: cabac=1 ref=3 deblock=1:0:0 analyse=0x3:0x113 me=hex subme=7 psy=1 psy_rd=1.00:0.00 mixed_ref=1 me_range=16 chroma_me=1 trellis=1 8x8dct=1 cqm=0 deadzone=21,11 fast_pskip=1 chroma_qp_offset=4 threads=18 lookahead_threads=3 sliced_threads=0 nr=0 decimate=1 interlaced=0 bluray_compat=0 constrained_intra=0 bframes=3 b_pyramid=2 b_adapt=1 b_bias=0 direct=1 weightb=1 open_gop=0 weightp=2 keyint=250 keyint_min=1 scenecut=40 intra_refresh=0 rc_lookahead=40 rc=crf mbtree=1 crf=23.0 qcomp=0.60 qpmin=0 qpmax=69 qpstep=4 ip_ratio=1.40 aq=1:1.00
Output #0, mp4, to 'output.mp4':
  Metadata:
    encoder         : Lavf60.16.100
  Stream #0:0: Video: h264 (avc1 / 0x31637661), yuvj444p(pc, bt470bg/unknown/unknown, progressive), 596x599, q=2-31, 1 fps, 16384 tbn
    Metadata:
      encoder         : Lavc60.31.102 libx264
    Side data:
      cpb: bitrate max/min/avg: 0/0/0 buffer size: 0 vbv_delay: N/A
  Stream #0:1: Audio: aac (LC) (mp4a / 0x6134706D), 44100 Hz, stereo, fltp, 128 kb/s
    Metadata:
      encoder         : Lavc60.31.102 aac
[out#0/mp4 @ 0x64f136c7d000] video:452kB audio:4697kB subtitle:0kB other streams:0kB global headers:0kB muxing overhead: 1.145771%
frame=  298 fps= 44 q=-1.0 Lsize=    5208kB time=00:04:58.30 bitrate= 143.0kbits/s speed=43.9x    
[libx264 @ 0x64f136c7eb80] frame I:2     Avg QP: 7.26  size:223602
[libx264 @ 0x64f136c7eb80] frame P:75    Avg QP: 8.62  size:   132
[libx264 @ 0x64f136c7eb80] frame B:221   Avg QP:17.33  size:    23
[libx264 @ 0x64f136c7eb80] consecutive B-frames:  1.0%  0.0%  1.0% 98.0%
[libx264 @ 0x64f136c7eb80] mb I  I16..4:  0.4% 91.6%  8.1%
[libx264 @ 0x64f136c7eb80] mb P  I16..4:  0.0%  0.0%  0.0%  P16..4:  2.3%  0.0%  0.0%  0.0%  0.0%    skip:97.7%
[libx264 @ 0x64f136c7eb80] mb B  I16..4:  0.0%  0.0%  0.0%  B16..8:  0.0%  0.0%  0.0%  direct: 0.0%  skip:100.0%  L0: 8.3% L1:91.7% BI: 0.0%
[libx264 @ 0x64f136c7eb80] 8x8 transform intra:91.6% inter:98.7%
[libx264 @ 0x64f136c7eb80] coded y,u,v intra: 98.6% 97.1% 97.2% inter: 0.1% 0.1% 0.1%
[libx264 @ 0x64f136c7eb80] i16 v,h,dc,p:  9%  0% 73% 18%
[libx264 @ 0x64f136c7eb80] i8 v,h,dc,ddl,ddr,vr,hd,vl,hu: 61% 31%  5%  1%  0%  1%  0%  1%  0%
[libx264 @ 0x64f136c7eb80] i4 v,h,dc,ddl,ddr,vr,hd,vl,hu: 22% 30%  9%  7%  7%  8%  4%  8%  5%
[libx264 @ 0x64f136c7eb80] Weighted P-Frames: Y:0.0% UV:0.0%
[libx264 @ 0x64f136c7eb80] ref P L0: 98.0%  0.0%  1.5%  0.4%
[libx264 @ 0x64f136c7eb80] ref B L0: 53.8% 46.2%
The file output.mp4 has been generated.
[libx264 @ 0x64f136c7eb80] kb/s:12.40
[aac @ 0x64f136ca6ec0] Qavg: 1208.003
$ 
```
