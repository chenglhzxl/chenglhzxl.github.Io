## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/chenglhzxl/chenglhzxl.github.Io/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/chenglhzxl/chenglhzxl.github.Io/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.


# Welcome to my Blog

## 2017年11月21日
### js验证年月日(yyyy-mm-dd)格式

``` bash
    function dateCheck(dateString){
        var result = dateString.match(/^(\d{1,4})(-|\/)(\d{1,2})\2(\d{1,2})$/);
        if(result == null){
            return false;
        }
        var d = new Date(result[1],result[3]-1,$result[4])
        return d.getFullYear()==result[1]&&(d.getMonth()+1)==result[3]&&d.getDate()==result[4];
    }
```

### js验证年月日(yyyymm)格式
``` bash
   function dateCheck(dateString) {
           var result = dateString.match(/^(\d{1,4})(\d{1,2})$/);
           if (result == null) {
               return false;
           }
           var d = new Date(result[1], result[2] - 1);
           return (d.getFullYear() == result[1] && (d.getMonth() + 1) == result[2]);
       }

```
