
.PHONY: all clean

#input files
PNG    	= $(wildcard *.png)

#output files
PNG2JPG	= $(patsubst %.png, %-thumb.jpg, $(PNG))

all: $(PNG2JPG) 

%-thumb.jpg: %.png 
	convert $< -resize x200 $@

clean:
	rm -f $(PNG2JPG)
