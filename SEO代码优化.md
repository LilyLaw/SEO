## SEO 和 网站代码层面优化

### 语义化代码

说白了就是多用语义化标签，在适当的位置用适当的标签

先择几个重要的讲一讲

1. ```<a>``` 
	- 加上title属性就是链接的说明。但我在html5规范里没有看到title属性 https://developer.mozilla.org/en-US/docs/Web/HTML/Element/a ，只看到下面这句话。那html5 有没有把这个属性废弃呢？ html4 标准也没看到啊。。。
	> HTML 3.2 defines only the name, href, rel, rev, and title attributes.

	- 加上rel属性，指明目标对象到链接对象的关系，如果指到了外链接，要用nofollow属性值指示搜索引擎不必去追了。

2. ```<h1>```
	搜索引擎优先搜索h1标签的内容，将h1标签看做最重要。
	正文标题用h1，副标题用h2，其他地方不要滥用标签。

3. ```<p>``` 和 ```<br />```
	p 是段落标签，注意其中不能再使用块级标签
	**br 标签是换行，但只能用于文本内换行。**
	
4. ```<caption>```
	专门用来写表格标题的
	``` html
	<table>
		<caption>company staff</caption>
		<thead>
			<tr>
				<td>name</td>
				<td>age</td>
			</tr>
		</thead>
		<tbody>
			<tr>
				<td>lily</td>
				<td>11</td>
			</tr>
			<tr>
				<td>jack</td>
				<td>12</td>
			</tr>
			<tr>
				<td>tom</td>
				<td>13</td>
			</tr>
		</tbody>
	</table>
	```

5. ```<img>```
	应尽量使用alt说明，搜索引擎不能识别图片内容，alt属性可以告诉搜索引擎这个图片是什么。
	
6. ```<strong>```,```<em>```和```<b>```,```<i>```
	```<strong>``` 在搜索引擎中权重较高，用于突出关键词等重要内容。	```<b>``` 显示效果和```<strong>``` 一样，但与SEO无关，所以若仅做样式修饰的话建议使用```<b>``` ，与SEO有关建议使用```<strong>``` 
	
	```<em>``` 和 ```<i>```与上述情况一样，与SEO相关用```<em>``` ，与SEO无关用```<i>```。

7. 重要代码放在前面
	代码读取是从上到下，尽量让搜索引擎尽快读取到重要内容。
	
8. 重要内容不要用JS输出
	搜索引擎无法识别js内容。

9. 尽量少使用iframe框架
	搜索引擎一般不会读取iframe框架内的内容。

10. 尽量少使用display：none
	搜索引擎会过滤掉display：none元素中的内容。

