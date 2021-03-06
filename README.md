
注意事项：
使用前请仔细阅读“scutthesis说明.pdf”、“sample_test.pdf”和attachment里面的撰写规范文档。
编译时如果提示缺乏字体，请按照attachment里面的字体（右键安装即可）。

建议使用texlive2018。如果是用texlive2019（windows）编译，会出现brokenpipe提示出错。这时可以按R同学找的方法更改scutthesis.cls第445行中的内容，将
\includepdf[pages=-]{thesis_cover.pdf}
换成
\includepdf[pages={1-5,{},7-8}]{thesis_cover.pdf}
详情请看：https://wenda.latexstudio.net/q-1962.html。
或按Y同学提供的信息，这时可以更改scutthesis.cls第445行中的内容，将\includepdf改成\includegraphics（但是pdf模板超过5页时，据说首页PDF模板的左右对齐格式会有些不合规范）。


-------------------------------------------------------
-------------------------------------------------------
本文档基于《华南理工大学学位论文Latex/Lyx模板》（来自https://github.com/alwintsui/scutthesis，详情请看其相关介绍说明），增删内容如下：
-------2019.11.08
1.	补充了部分图、表和公式的演示例子。
2.	修改了scutthesis.bst，使得即便reference.bib里面有多余未引用条目，在Windows 的Texlive（2018）下依然能够顺利编译通过。
3.	修改了结论在chapterx命令下，偶数页显示上一章标题的错误。
4.	修改了附录中图、表和公式接着正文章节序号编号的错误。
5.	修改了在Windows下致谢最后名称和日期没有右对齐的格式。
-------2020.03.29
6.	修改了参考文献中会议类型文献出现两个文献标记的错误。
7.	修改了当参考文献包含doi字段时正文无法生成参考文献列表的错误。
