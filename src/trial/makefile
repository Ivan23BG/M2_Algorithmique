THEMES = light dark
BUILD_DIR = build

.PHONY: all clean

all:
	@mkdir -p $(BUILD_DIR)
	@for theme in $(THEMES); do \
		pdflatex -jobname=$(BUILD_DIR)/academic_$${theme} "\def\THEME{$${theme}}\input{main.tex}"; \
	done

clean:
	rm -rf $(BUILD_DIR)