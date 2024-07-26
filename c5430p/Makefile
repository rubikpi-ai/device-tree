%:
	${CC} -undef -x assembler-with-cpp $(shell pwd)/$@.dtso -I ${KERNEL_INCLUDE} -E -o $(shell pwd)/$@.dtso.preprocessed
	${DTC} -O dtb -o $(shell pwd)/$@.dtbo $(shell pwd)/$@.dtso.preprocessed

clean:
	rm -rf *.preprocessed
