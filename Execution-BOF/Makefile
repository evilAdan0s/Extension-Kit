all: bof

clean:
	@(rm -f _bin/* && echo '[*] cleaned')

bof:
	@(mkdir _bin 2>/dev/null) && echo '[+] creating _bin' || echo '[*] _bin exists'
	@(x86_64-w64-mingw32-gcc -w -Wno-incompatible-pointer-types -o _bin/execute-assembly.x64.o -I . -Os -s -c execute-assembly/inlineExecute-Assembly.c && x86_64-w64-mingw32-strip --strip-unneeded _bin/execute-assembly.x64.o) && echo '[*] execute-assembly' || echo '[!] execute-assembly build failed'
