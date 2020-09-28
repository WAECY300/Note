# table

	在表格内，通过行与列来创建表格，tr代表行，td代表列，也叫单元格
>
>
>创建一个2列的表格

```html
<tale>
      <tr>
      	<td></td>
      	<td></td>
      </tr>
      
      <tr>
        <td></td>
        <td></td>
      </tr>
</table>
```



默认状态下，table制作出来的表格没有基本表格出现的边框线等，所以，我们可以为table添加如下的属性`table`

## border属性

table的border属性用于为table元素添加边框，值为数字，单位可有可无

```html
<table border="1">
 <tr>
     <td>1</td>
     <td>2</td>
 </tr>
```

border只作用于table和td这俩个元素，不能为tr提供边框效果.

## width和height

```
<table border="1" width="800px" height="400px">
  <tr>
   <td>1</td>
   <td>2</td>
  </tr>
</table>
```

# align水平排列属性

>align = 'left/center/right'

​       该属性对于table/tr/td都存有不同的显示效果

​		对于table而言。align的值，改变了当前table表格的水平位置

​		对于tr而言。align的值，改变当前行内所有单元格的值的位置

​		对于td而言。align的值。改变当前单元格的值的位置


# valign 垂直排列属性

>
>
>valign = 'top/middle/bottom'

​       对于tr而言。valign的值，改变当前行内所有所有单元格的值的位置

​		对于td而言。valign的值，改变当前单元格的值的位置

​     td 改变宽高   tr改变行高

