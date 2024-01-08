# Cangjie5

[傳統漢字版說明](https://github.com/Jackchows/Cangjie5/blob/master/README.md)

相关项目：[Arthurmcarthur/Cangjie3-Plus](https://github.com/Arthurmcarthur/Cangjie3-Plus)

原码表为[「仓颉平台 2012」](https://chinesecj.com/forum/forum.php?mod=viewthread&tid=2596)的「五仓世纪」码表。

## 下载
[按此](https://github.com/Jackchows/Cangjie5/releases/download/v3.0/RimeData_20231117_Cangjie5.7z)下载适用于RIME的输入法方案文档。<br />
[按此](https://github.com/Jackchows/Cangjie5/releases/download/v3.0/MSCJData_20231117_Cangjie5.7z)下载适用于替换微软仓颉码表的文档。（使用说明见[此处](http://www.chinesecj.com/forum/forum.php?mod=viewthread&tid=194346)）

## 目标

**本项目参考官方资料对码表进行修改，可能与其他常见仓颉输入法软件存在差异，使用前务必阅读[说明](https://github.com/Jackchows/Cangjie5/blob/master/change_summary.md#%E4%B8%BB%E8%A6%81%E6%94%B9%E7%A2%BC%E8%AA%AA%E6%98%8E%E5%8F%8A%E7%88%AD%E8%AD%B0%E5%8F%96%E7%A2%BC)。**<br />
1. 所称「官方资料」，包括：
	1. 《第五代仓颉输入法手册》（松岗，1993、文化传信，1999、博硕，2006）
	2. [「汉文库典」](http://chidic.eduhk.hk/)网站
	3. 朱邦复工作室《内码对照表》（含2003版五代、六代编码）
	4. 《零壹中文电脑丛书之八 仓颉第三代中文字母输入法》（全华，1984）、《零壹中文电脑丛书之九 增订版仓颉第三代中文输入法》（全华，1991）
	5. 《零壹中文电脑丛书之七 标准仓颉第二代中文输入法》（全华，1983）
	6. 沈红莲女士之信函
2. 本项目：
	1. **(✓)意图**　修改字码以贴近官方资料
	2. **(✗)无意**　修改或解释官方码表中被认为不符合仓颉输入法规则的部分（明显的笔误除外）
	3. **(✓)意图**　完善字形兼容（参考官方码表为主，适当添加各地字形）
	4. **(✗)无意**　兼容全部旧字形、中国大陆、香港、台湾、日本、韩国、越南字形
	5. **(✓)意图**　根据个人主观理解制作一份码表，为大家提供一个选择
	6. **(✗)无意**　满足所有人的需求

## 内容

- **[Cangjie5.txt](https://github.com/Jackchows/Cangjie5/blob/master/Cangjie5.txt)**<br />
码表。**一般排序**，综合考虑字频及繁简（**部分常用简化字可能排列于传统汉字前**）。<br />
收录中日韩统一表意文字（基本区至扩展I区）字符、[兼容汉字](https://zh.wikipedia.org/wiki/%E4%B8%AD%E6%97%A5%E9%9F%93%E7%9B%B8%E5%AE%B9%E8%A1%A8%E6%84%8F%E6%96%87%E5%AD%97)区中视作统一汉字的十二个字符，以及官方码表中收录的符号。<br />
另外收录兼容汉字、部首、笔画以及其他一些形似汉字的符号。为避免与常规汉字混淆，**此部分字符编码以「z」开头**（兼容汉字「zc」，部首「zr」，笔画「zs」，表意文字描述字符「zi」，算筹符号「zn」，其他符号「zf」）。
- **[Cangjie5_TC.txt](https://github.com/Jackchows/Cangjie5/blob/master/Cangjie5_TC.txt)**<br />
码表。**传统汉字优先**（限《常用国字标准字体表》、《次常用国字标准字体表》及《常用字字形表》范围）。<br />
收字范围与 Cangjie5.txt 相同。
- **[Cangjie5_SC.txt](https://github.com/Jackchows/Cangjie5/blob/master/Cangjie5_SC.txt)**<br />
码表。**简化字优先**（限《通用规范汉字表》范围）。<br />
收字范围与 Cangjie5.txt 相同。
- **[Cangjie5_supplement.txt](https://github.com/Jackchows/Cangjie5/blob/master/Cangjie5_supplement.txt)**<br />
码表。收录兼容汉字、部首、笔画以及其他一些形似汉字的符号。此表按原始编码收录，编码不以「z」开头。<br />
- **[change_summary.md](https://github.com/Jackchows/Cangjie5/blob/master/change_summary.md)    ※请首先阅读此文档。**<br />
总体说明，包括取码争议、字形兼容、重码字排序调整说明。
- **[change_details.log](https://github.com/Jackchows/Cangjie5/blob/master/change_details.log)**<br />
码表的详细编辑记录。
- **[Cangjie5_special.txt](https://github.com/Jackchows/Cangjie5/blob/master/Cangjie5_special.txt)**<br />
码表。**特别版本**，收录主流系统可以直接显示的字符，包括：中日韩统一表意文字基本区（除去 U+9FD1 至 U+9FFF）、扩展A区（除去 U+4DB6 至 U+4DBF）、兼容汉字区中视作统一汉字的十二个字符、《通用规范汉字表》、《香港增补字符集—2016》（HKSCS）。<br />
另外，[Change_summary.md#字形问题](https://github.com/Jackchows/Cangjie5/blob/master/change_summary.md#%E5%AD%97%E5%BD%A2%E5%95%8F%E9%A1%8C) 中列出的多种字形，此表会尽数收录。<br />
此码表与前面几份码表更新可能不同步。

## 反馈

若发现错误，可在此处[反馈](https://github.com/Jackchows/Cangjie5/issues/new)。
多谢！

## 注释

注1：目前找到的最早版本是1991年9月出版的第十五版，初版时间可能更早。
