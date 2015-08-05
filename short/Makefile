define my_rule
target/$1/$2.txt: source/$1/$2.png
	mkdir -p $$(dir $$@)
	touch $$@
endef

$(foreach X,A B C,\
	$(foreach Y,1 2 3,\
		$(eval $(call my_rule,$(X),$(Y)))))
