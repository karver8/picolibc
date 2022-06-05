#
# SPDX-License-Identifier: BSD-3-Clause
#
# Copyright © 2022 Keith Packard
#
# Redistribution and use in source and binary forms, with or without
# modification, are permitted provided that the following conditions
# are met:
#
# 1. Redistributions of source code must retain the above copyright
#    notice, this list of conditions and the following disclaimer.
#
# 2. Redistributions in binary form must reproduce the above
#    copyright notice, this list of conditions and the following
#    disclaimer in the documentation and/or other materials provided
#    with the distribution.
#
# 3. Neither the name of the copyright holder nor the names of its
#    contributors may be used to endorse or promote products derived
#    from this software without specific prior written permission.
#
# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
# "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT
# LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS
# FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE
# COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT,
# INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
# (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
# SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
# HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,
# STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
# ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED
# OF THE POSSIBILITY OF SUCH DAMAGE.
#
picolibc_sources(
asiprintf.c   
asniprintf.c  
asnprintf.c   
asprintf.c    
clearerr.c    
clearerr_u.c
diprintf.c    
dprintf.c     
fclose.c      
# fcloseall.c
fdopen.c
feof.c
feof_u.c
ferror.c
ferror_u.c
# fflush.c
# fflush_u.c
fgetc.c
fgetc_u.c
fgetpos.c
fgets.c
fgets_u.c
fgetwc.c
fgetwc_u.c
fgetws.c
fgetws_u.c
fileno.c
fileno_u.c
# findfp.c
fiprintf.c
fiscanf.c
flags.c
fmemopen.c
fopen.c
fopencookie.c
fprintf.c
fpurge.c
fputc.c
fputc_u.c
fputs.c
fputs_u.c
fputwc.c
fputwc_u.c
fputws.c
fputws_u.c
fread.c
fread_u.c
freopen.c
fscanf.c
fseek.c
fseeko.c
fsetlocking.c
fsetpos.c
ftell.c
ftello.c
funopen.c
fvwrite.c
fwalk.c
fwide.c
# fwprintf.c
fwrite.c
fwrite_u.c
# fwscanf.c
getc.c
getc_u.c
getchar.c
getchar_u.c
getdelim.c
getline.c
gets.c
# getw.c
# getwc.c
# getwc_u.c
# getwchar.c
# getwchar_u.c
iprintf.c
iscanf.c
makebuf.c
mktemp.c
nano-svfprintf.c
nano-svfscanf.c
nano-vfprintf.c
nano-vfprintf_float.c
nano-vfprintf_i.c
nano-vfscanf.c
nano-vfscanf_float.c
nano-vfscanf_i.c
open_memstream.c
# perror.c
printf.c
putc.c
putc_u.c
putchar.c
putchar_u.c
puts.c
# putw.c
# putwc.c
# putwc_u.c
# putwchar.c
# putwchar_u.c
# refill.c
remove.c
rename.c
rewind.c
rget.c
scanf.c
sccl.c
setbuf.c
setbuffer.c
setlinebuf.c
setvbuf.c
siprintf.c
siscanf.c
sniprintf.c
snprintf.c
sprintf.c
sscanf.c
stdio.c
stdio_ext.c
svfiprintf.c
svfiscanf.c
# svfiwprintf.c
# svfiwscanf.c
# svfprintf.c
# svfscanf.c
# svfwprintf.c
# svfwscanf.c
# swprintf.c
# swscanf.c
tmpfile.c
tmpnam.c
ungetc.c
ungetwc.c
vasiprintf.c
vasniprintf.c
vasnprintf.c
vasprintf.c
vdiprintf.c
vdprintf.c
vfiprintf.c
vfiscanf.c
# vfiwprintf.c
# vfiwscanf.c
# vfprintf.c
# vfscanf.c
# vfwprintf.c
# vfwscanf.c
viprintf.c
viscanf.c
vprintf.c
vscanf.c
vsiprintf.c
vsiscanf.c
vsniprintf.c
vsnprintf.c
vsprintf.c
vsscanf.c
# vswprintf.c
# vswscanf.c
# vwprintf.c
# vwscanf.c
wbuf.c
# wprintf.c
# wscanf.c
wsetup.c
  )

if(POSIX_CONSOLE)
  picolibc_sources(
    posixiob.c
    )
endif()

picolibc_headers(""
 floatio.h
 fvwrite.h
 local.h
 nano-vfprintf_local.h
 nano-vfscanf_local.h
 stdio.h
 stdio_ext.h
 vfieeefp.h
)
