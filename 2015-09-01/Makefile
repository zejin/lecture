.PHONY: submit clean

submit: centroid
	qsub centroid.pbs

centroid: centroid.c centroid.h centroid_timer.c
	gcc -O0 -fopenmp -o centroid centroid.c centroid_timer.c

clean:
	rm -f centroid
	rm *.o*
