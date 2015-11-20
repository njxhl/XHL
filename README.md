# 南京新货郎电子商务有限公司 官网

## 1.data里面的dsj.json   gsdt.json   gsgg.json

 - dsj.json 用于大事记列表页面的展示
 - gsdt.json 用于公司动态列表页面的展示
 - gsgg.json 用于公司公告列表页面的展示
 
 \* 列表页面json数据格式说明
 
    {
        "title" : "这里是标题",
        "year" : "年",
        "month" : "月",
        "day" : "日"
        "articleUrl":"这里是文章所在文件夹名",
        "previewImg":"这里是预览图片的路径",
        "content":"这里是文章的大致内容,或一部分文字内容"
    }
    

## 2.data/2015/11/13/1/1.json 表示data/2015/11/13/1日第一篇文章所在目录,文件名为1.json,其他图片为文章内引用图片

\* 文章页面json数据格式说明

    {
        "baseUrl" : "文章所在基本路径",       例:/XHL/data/dsj/2015/11/13/1
        "title" : "文章标题",
        "time" : "文章发布时间",
        "author" : "作者",
        "content" : 
        [
            {
                "type" : "数据类型",        p表示段落,img表示图片,strong表示图片下方说明
                "content" : "内容"         如果是文字,直接写,如果是图片,写图片名
            },
            {
                "type" : "数据类型",        
                "content" : "内容"         
            }
            ……                             …… 表示,可以加多个,格式与上面相同
        ],
        "keywords" : 
        [
            {
                "content" : "关键字",
                "url" : "链接路径"
            }
            ……
        ],
        "pre" : "上一篇文章链接",
        "preContent" : "上一篇文章标题",
        "next" : "下一篇文章链接",
        "nextContent" : "下一篇文章标题"
    }


   