# \# 一级标题
## \#\# 二级标题
### \#\#\# 三级标题
### 多一个\#则字体小一号
# 1、如何输出空格
## \&nbsp; &nbsp;space
## \&ensp; &ensp;半角
## \&emsp; &emsp;全角
## 如何创建表格
### 采用html的方式
<table>
<tr>
<th>表头</th>
</tr>
<tr>
<td>下一行</td>
</tr>
</table>

# 2、如何打出希腊字母
<p>希腊字母</p> 
<table><thead><tr><th>大写</th><th>Markdown</th><th>小写</th><th>Markdown</th></tr></thead><tbody><tr><td>A</td><td>A</td><td>α</td><td>\alpha</td></tr><tr><td>B</td><td>B</td><td>β</td><td>\beta</td></tr><tr><td>Γ</td><td>\Gamma</td><td>γ</td><td>\gamma</td></tr><tr><td>Δ</td><td>\Delta</td><td>δ</td><td>\delta</td></tr><tr><td>E</td><td>E</td><td>ϵ</td><td>\epsilon</td></tr><tr><td> </td><td> </td><td>ε</td><td>\varepsilon</td></tr><tr><td>Z</td><td>Z</td><td>ζ</td><td>\zeta</td></tr><tr><td>H</td><td>H</td><td>η</td><td>\eta</td></tr><tr><td>Θ</td><td>\Theta</td><td>θ</td><td>\theta</td></tr><tr><td>I</td><td>I</td><td>ι</td><td>\iota</td></tr><tr><td>K</td><td>K</td><td>κ</td><td>\kappa</td></tr><tr><td>Λ</td><td>\Lambda</td><td>λ</td><td>\lambda</td></tr><tr><td>M</td><td>M</td><td>μ</td><td>\mu</td></tr><tr><td>N</td><td>N</td><td>ν</td><td>\nu</td></tr><tr><td>Ξ</td><td>\Xi</td><td>ξ</td><td>\xi</td></tr><tr><td>O</td><td>O</td><td>ο</td><td>\omicron</td></tr><tr><td>Π</td><td>\Pi</td><td>π</td><td>\pi</td></tr><tr><td>P</td><td>P</td><td>ρ</td><td>\rho</td></tr><tr><td>Σ</td><td>\Sigma</td><td>σ</td><td>\sigma</td></tr><tr><td>T</td><td>T</td><td>τ</td><td>\tau</td></tr><tr><td>Υ</td><td>\Upsilon</td><td>υ</td><td>\upsilon</td></tr><tr><td>Φ</td><td>\Phi</td><td>ϕ</td><td>\phi</td></tr><tr><td> </td><td> </td><td>φ</td><td>\varphi</td></tr><tr><td>X</td><td>X</td><td>χ</td><td>\chi</td></tr><tr><td>Ψ</td><td>\Psi</td><td>ψ</td><td>\psi</td></tr><tr><td>Ω</td><td>\Omega</td><td>ω</td><td>\omega</td></tr></tbody></table>
<p>扩展&#xff1a;</p> 
<p><strong>上/下标</strong></p> 
<table><thead><tr><th>算式</th><th>Markdown</th></tr></thead><tbody><tr><td> </td><td>x^2</td></tr><tr><td> </td><td>y_1</td></tr></tbody></table>
<p><strong>分式</strong></p> 
<table><thead><tr><th>算式</th><th>Markdown</th></tr></thead><tbody><tr><td>1/2</td><td>1/2</td></tr><tr><td>1/2</td><td>\frac{1}{2}</td></tr></tbody></table>
<p><strong>省略号</strong></p> 
<table><thead><tr><th>省略号</th><th>Markdown</th></tr></thead><tbody><tr><td>⋯</td><td>\cdots</td></tr></tbody></table>
<p><strong>开根号</strong></p> 
<table><thead><tr><th>算式</th><th>Markdown</th></tr></thead><tbody><tr><td></td><td>\sqrt{2}</td></tr></tbody></table>
<p><strong>矢量</strong></p> 
<table><thead><tr><th>算式</th><th>Markdown</th></tr></thead><tbody><tr><td></td><td>\vec{a}</td></tr></tbody></table>
<p><strong>积分</strong></p> 
<table><thead><tr><th>算式</th><th>Markdown</th></tr></thead><tbody><tr><td>∫xdx</td><td>\int{x}dx</td></tr><tr><td>∫12xdx</td><td>\int_{1}^{2}{x}dx</td></tr></tbody></table>
<p><strong>极限</strong></p> 
<table><thead><tr><th>算式</th><th>Markdown</th></tr></thead><tbody><tr><td>lim⁡a&#43;b</td><td>\lim{a&#43;b}</td></tr><tr><td>lim⁡n→&#43;∞</td><td>\lim_{n\rightarrow&#43;\infty}</td></tr></tbody></table>
<p><strong>累加</strong></p> 
<table><thead><tr><th>算式</th><th>Markdown</th></tr></thead><tbody><tr><td>∑a</td><td>\sum{a}</td></tr><tr><td>∑n&#61;1100an</td><td>\sum_{n&#61;1}^{100}{a_n}</td></tr></tbody></table>
<p><strong>累乘</strong></p> 
<table><thead><tr><th>算式</th><th>Markdown</th></tr></thead><tbody><tr><td>∏x</td><td>\prod{x}</td></tr><tr><td>∏n&#61;199xn</td><td>\prod_{n&#61;1}^{99}{x_n}</td></tr></tbody></table>
<p><strong>三角函数</strong></p> 
<table><thead><tr><th>三角函数</th><th>Markdown</th></tr></thead><tbody><tr><td>sin⁡</td><td>\sin</td></tr></tbody></table>
<p><strong>对数函数</strong></p> 
<table><thead><tr><th>算式</th><th>Markdown</th></tr></thead><tbody><tr><td>ln⁡2</td><td>\ln2</td></tr><tr><td>log⁡28</td><td>\log_28</td></tr><tr><td>lg⁡10</td><td>\lg10</td></tr></tbody></table>
<p><strong>关系运算符</strong></p> 
<table><thead><tr><th>运算符</th><th>Markdown</th></tr></thead><tbody><tr><td>±</td><td>\pm</td></tr><tr><td>\times</td><td>\times</td></tr><tr><td>⋅</td><td>\cdot</td></tr><tr><td>÷</td><td>\div</td></tr><tr><td>\neq</td><td>\neq</td></tr><tr><td>≡</td><td>\equiv</td></tr><tr><td>≤</td><td>\leq</td></tr><tr><td>≥</td><td>\geq</td></tr></tbody></table>
<p><strong>其它特殊字符</strong></p> 
<table><thead><tr><th>符号</th><th>Markdown</th></tr></thead><tbody><tr><td>∀</td><td>\forall</td></tr><tr><td>∞</td><td>\infty</td></tr><tr><td>∅</td><td>\emptyset</td></tr><tr><td>∃</td><td>\exists</td></tr><tr><td>∇</td><td>\nabla</td></tr><tr><td>⊥</td><td>\bot</td></tr><tr><td>∠</td><td>\angle</td></tr><tr><td>∵</td><td>\because</td></tr><tr><td>∴</td><td>\therefore</td></tr></tbody></table>
