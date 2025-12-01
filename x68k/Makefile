PNG=OSChiroshima.png

b:
	#fastfetch --raw test.sixel --logo-width 21 --logo-height 20 --logo-padding-top 2
	fastfetch --raw test.sixel --logo-width 70 --logo-height 20 --logo-padding-top 10 
a:
	#chafa -s 500x10  ${PNG} > test.sixel
	chafa  ${PNG} > test.sixel

install:
	pkg_add chafa
	pkg_add fastfetch
