# 本仓库是关于毕业设计的前后端实现

Category：# 一共分为三阶段完成
    一：前期设计

    二：中期

    三：最终完成

File Struction:
    ——|
      |——readme.md  项目概述和文档
      |——pic        测试文件的文件夹
      |  |Test_ooxml.docx—>Test_ooxml.zip
      |  | exact and the yellow mean dir, other means file
      |   OOXML_TestFile
            _rels
                .rels
                ｜ 连接app.xml和core.xml

            docProps
            ｜ 文档属性
                app.xml
                ｜ 配置文件，关于文档的模板版本、页数、应用、安全性、行段落、空等等【细节待补全】
                core.xml
                ｜ 描述文件作者、关键词、修改时间和人、版本和时间信息。

            word
                _rels
                ｜ 一个part依赖于其他part，为这个part创建的目录
                    document.xml.rels
                    ｜ 定义了 document.xml 和样式、页眉、页脚等 Part 间的关系

                theme
                    theme1.xml

                document.xml
                ｜ 文档正文布局和具体内容
                ｜ 主节点<w:document>表示文档本身，<w:body>表示内容体，其内包含<w:p>表示一个自然段落，而嵌套在<w:body>中的<w:sectPr>定义了页面维度。<w:rsidR>是一些标签的属性，意为修订标识符。所有段落和段落中的内容应有相同的属性值，如若不然表明段落被重新编辑过。<w:rsidRPr>是类似的，用来跟踪编辑在修订时字符或字形是否发生过改变。<w:p>标签包含一些<w:r>标签，一个<w:r>标签所包含的连续的字符串都具有完全相同的属性，如中文或英文字符字符串就会被分配到不同的标签中。对于同一种文字，如果它们的一些属性例如粗细程度、是否倾斜、是否有下划线等有所不同的时候也会用<w:r>标签进行分割并标记，并且会含有一个修改标记的属性<w:rsidRPr>。<w:r>的子标签<w:t>代表文字内容，其内包含一段字符串。<w:r>的子标签<w:color>代表当前标签内包含的文字拥有的相同的颜色，其颜色值<w:r>为标签下<w:val>标签的值，为十六进制的 RGB 格式。
                fontTable.xml
                settings.xml
                styles.xml
                webSettings.xml

            [Content_Types].xml
            ｜ 文档中的媒体类型信息——text、pictrue、
            test.ooxml
      |——code    代码文件

