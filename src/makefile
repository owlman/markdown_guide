# 作者：owlman
# 时间：2018年10月22日
# 作用：将markdown文件转换成docx格式

src = $(shell find ./ -name "*.md")
docx = $(src:%.md=../docx/%.docx)

all: $(docx)
	ls -l ../docx

../docx/%.docx:%.md
	pandoc -f markdown+tex_math_dollars -t docx $< -o $@  --latex-engine=xelatex

clean:
	rm -rf $(docx)