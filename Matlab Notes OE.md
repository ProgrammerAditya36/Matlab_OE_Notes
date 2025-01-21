---


---

<h1 id="class-2">Class 2</h1>
<pre class=" language-matlab"><code class="prism  language-matlab">clc<span class="token punctuation">;</span>clear<span class="token punctuation">;</span>
x <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">1</span><span class="token operator">:</span><span class="token number">2</span><span class="token operator">:</span><span class="token number">9</span><span class="token punctuation">;</span><span class="token number">2</span><span class="token operator">:</span><span class="token number">2</span><span class="token operator">:</span><span class="token number">10</span><span class="token punctuation">]</span><span class="token punctuation">;</span>
<span class="token comment">% x(end,1)</span>
<span class="token punctuation">[</span>m<span class="token punctuation">,</span>n<span class="token punctuation">]</span> <span class="token operator">=</span> <span class="token function">size</span><span class="token punctuation">(</span>x<span class="token punctuation">)</span><span class="token punctuation">;</span>
 <span class="token keyword">for</span> <span class="token number">i</span><span class="token operator">=</span><span class="token number">1</span><span class="token operator">:</span>m
	 <span class="token keyword">for</span> <span class="token number">j</span><span class="token operator">=</span><span class="token number">1</span><span class="token operator">:</span>n
		 <span class="token function">disp</span><span class="token punctuation">(</span><span class="token function">x</span><span class="token punctuation">(</span><span class="token number">i</span><span class="token punctuation">,</span><span class="token number">j</span><span class="token punctuation">)</span><span class="token punctuation">)</span> <span class="token comment">%() for printing</span>
	<span class="token keyword">end</span>
 <span class="token keyword">end</span>

<span class="token function">disp</span><span class="token punctuation">(</span><span class="token function">x</span><span class="token punctuation">(</span><span class="token number">1</span><span class="token operator">:</span><span class="token keyword">end</span><span class="token punctuation">,</span> <span class="token number">3</span><span class="token operator">:</span><span class="token keyword">end</span><span class="token punctuation">)</span><span class="token punctuation">)</span>
x<span class="token operator">'</span> <span class="token comment">% Transpose</span>
</code></pre>
<h1 id="class-3">Class 3</h1>
<p>17/01/2025</p>
<pre class=" language-matlab"><code class="prism  language-matlab"><span class="token function">zeros</span><span class="token punctuation">(</span><span class="token number">2</span><span class="token punctuation">)</span> <span class="token comment">% 0 Matrix of dimension 2</span>
<span class="token function">ones</span><span class="token punctuation">(</span><span class="token number">2</span><span class="token punctuation">)</span> <span class="token comment">% 1 Matrix of dimension 3</span>
<span class="token function">eye</span><span class="token punctuation">(</span><span class="token number">2</span><span class="token punctuation">)</span> <span class="token comment">% Identity matrix</span>
<span class="token function">magic</span><span class="token punctuation">(</span><span class="token number">3</span><span class="token punctuation">)</span> <span class="token comment">%Magic square</span>
a <span class="token operator">=</span><span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">,</span><span class="token number">2</span><span class="token punctuation">,</span><span class="token number">4</span><span class="token punctuation">;</span><span class="token number">5</span><span class="token punctuation">,</span><span class="token number">6</span><span class="token punctuation">,</span><span class="token number">7</span><span class="token punctuation">;</span><span class="token number">8</span><span class="token punctuation">,</span><span class="token number">9</span><span class="token punctuation">,</span><span class="token number">10</span><span class="token punctuation">]</span>

a <span class="token operator">=</span>

     <span class="token number">1</span>     <span class="token number">2</span>     <span class="token number">4</span>
     <span class="token number">5</span>     <span class="token number">6</span>     <span class="token number">7</span>
     <span class="token number">8</span>     <span class="token number">9</span>    <span class="token number">10</span>

<span class="token operator">&gt;</span><span class="token operator">&gt;</span> <span class="token function">fliplr</span><span class="token punctuation">(</span>a<span class="token punctuation">)</span>

ans <span class="token operator">=</span>

     <span class="token number">4</span>     <span class="token number">2</span>     <span class="token number">1</span>
     <span class="token number">7</span>     <span class="token number">6</span>     <span class="token number">5</span>
    <span class="token number">10</span>     <span class="token number">9</span>     <span class="token number">8</span>

<span class="token operator">&gt;</span><span class="token operator">&gt;</span> <span class="token function">flipud</span><span class="token punctuation">(</span>a<span class="token punctuation">)</span>

ans <span class="token operator">=</span>

     <span class="token number">8</span>     <span class="token number">9</span>    <span class="token number">10</span>
     <span class="token number">5</span>     <span class="token number">6</span>     <span class="token number">7</span>
     <span class="token number">1</span>     <span class="token number">2</span>     <span class="token number">4</span>

<span class="token comment">% Square matrix multiplication</span>
 x <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">,</span><span class="token number">2</span><span class="token punctuation">,</span><span class="token number">3</span><span class="token punctuation">;</span><span class="token number">4</span><span class="token punctuation">,</span><span class="token number">5</span><span class="token punctuation">,</span><span class="token number">6</span><span class="token punctuation">;</span><span class="token number">7</span><span class="token punctuation">,</span><span class="token number">8</span><span class="token punctuation">,</span><span class="token number">9</span><span class="token punctuation">]</span>

x <span class="token operator">=</span>

     <span class="token number">1</span>     <span class="token number">2</span>     <span class="token number">3</span>
     <span class="token number">4</span>     <span class="token number">5</span>     <span class="token number">6</span>
     <span class="token number">7</span>     <span class="token number">8</span>     <span class="token number">9</span>

<span class="token operator">&gt;</span><span class="token operator">&gt;</span> x<span class="token operator">*</span>x

ans <span class="token operator">=</span>

    <span class="token number">30</span>    <span class="token number">36</span>    <span class="token number">42</span>
    <span class="token number">66</span>    <span class="token number">81</span>    <span class="token number">96</span>
   <span class="token number">102</span>   <span class="token number">126</span>   <span class="token number">150</span>

<span class="token comment">% Matrix multiplacation with transpose </span>
<span class="token operator">&gt;</span><span class="token operator">&gt;</span> y <span class="token operator">=</span> <span class="token number">1</span><span class="token operator">:</span><span class="token number">10</span>

y <span class="token operator">=</span>

     <span class="token number">1</span>     <span class="token number">2</span>     <span class="token number">3</span>     <span class="token number">4</span>     <span class="token number">5</span>     <span class="token number">6</span>     <span class="token number">7</span>     <span class="token number">8</span>     <span class="token number">9</span>    <span class="token number">10</span>

<span class="token operator">&gt;</span><span class="token operator">&gt;</span> y<span class="token operator">*</span>y<span class="token operator">'</span>

ans <span class="token operator">=</span>

   <span class="token number">385</span>

<span class="token comment">% Dot Operator (performs element by elemnt operation)</span>

x

x <span class="token operator">=</span>

     <span class="token number">1</span>     <span class="token number">2</span>     <span class="token number">3</span>
     <span class="token number">4</span>     <span class="token number">5</span>     <span class="token number">6</span>
     <span class="token number">7</span>     <span class="token number">8</span>     <span class="token number">9</span>

<span class="token operator">&gt;</span><span class="token operator">&gt;</span> y <span class="token operator">=</span> <span class="token function">magic</span><span class="token punctuation">(</span><span class="token number">3</span><span class="token punctuation">)</span>

y <span class="token operator">=</span>

     <span class="token number">8</span>     <span class="token number">1</span>     <span class="token number">6</span>
     <span class="token number">3</span>     <span class="token number">5</span>     <span class="token number">7</span>
     <span class="token number">4</span>     <span class="token number">9</span>     <span class="token number">2</span>

<span class="token operator">&gt;</span><span class="token operator">&gt;</span> x<span class="token operator">.*</span>y

ans <span class="token operator">=</span>

     <span class="token number">8</span>     <span class="token number">2</span>    <span class="token number">18</span>
    <span class="token number">12</span>    <span class="token number">25</span>    <span class="token number">42</span>
    <span class="token number">28</span>    <span class="token number">72</span>    <span class="token number">18</span>
 a <span class="token operator">=</span> x<span class="token operator">.*</span>y<span class="token punctuation">;</span>
<span class="token operator">&gt;</span><span class="token operator">&gt;</span> a<span class="token operator">./</span><span class="token number">3</span>

ans <span class="token operator">=</span>

    <span class="token number">2.6667</span>    <span class="token number">0.6667</span>    <span class="token number">6.0000</span>
    <span class="token number">4.0000</span>    <span class="token number">8.3333</span>   <span class="token number">14.0000</span>
    <span class="token number">9.3333</span>   <span class="token number">24.0000</span>    <span class="token number">6.0000</span>



<span class="token comment">% Concatenation</span>

c <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">1</span><span class="token operator">:</span><span class="token number">5</span><span class="token punctuation">]</span>

c <span class="token operator">=</span>

     <span class="token number">1</span>     <span class="token number">2</span>     <span class="token number">3</span>     <span class="token number">4</span>     <span class="token number">5</span>

<span class="token operator">&gt;</span><span class="token operator">&gt;</span> Ch <span class="token operator">=</span> <span class="token punctuation">[</span>c<span class="token punctuation">,</span>c<span class="token punctuation">]</span> <span class="token comment">% can use horzcat() too</span>

Ch <span class="token operator">=</span>

     <span class="token number">1</span>     <span class="token number">2</span>     <span class="token number">3</span>     <span class="token number">4</span>     <span class="token number">5</span>     <span class="token number">1</span>     <span class="token number">2</span>     <span class="token number">3</span>     <span class="token number">4</span>     <span class="token number">5</span>

<span class="token operator">&gt;</span><span class="token operator">&gt;</span> Cv <span class="token operator">=</span> <span class="token punctuation">[</span>c<span class="token punctuation">;</span>c<span class="token punctuation">]</span> <span class="token comment">% can use vertcat() too</span>

Cv <span class="token operator">=</span>

     <span class="token number">1</span>     <span class="token number">2</span>     <span class="token number">3</span>     <span class="token number">4</span>     <span class="token number">5</span>
     <span class="token number">1</span>     <span class="token number">2</span>     <span class="token number">3</span>     <span class="token number">4</span>     <span class="token number">5</span>


<span class="token comment">% Saving workspace and loading it</span>
<span class="token operator">&gt;</span><span class="token operator">&gt;</span> save matlab
<span class="token operator">&gt;</span><span class="token operator">&gt;</span> clear all
<span class="token operator">&gt;</span><span class="token operator">&gt;</span> load matlab

<span class="token comment">% only one variable</span>
<span class="token operator">&gt;</span><span class="token operator">&gt;</span> k <span class="token operator">=</span> <span class="token number">20</span>
<span class="token operator">&gt;</span><span class="token operator">&gt;</span> save justk k


</code></pre>
<p><a href="https://in.mathworks.com/help/phased/ref/physconst.html">Physical Constants</a></p>
<h1 id="class-4">Class 4</h1>
<h2 id="cell-array">Cell Array</h2>
<pre class=" language-matlab"><code class="prism  language-matlab"><span class="token operator">&gt;</span><span class="token operator">&gt;</span> c <span class="token operator">=</span> <span class="token punctuation">{</span><span class="token string">'2017-08-16'</span><span class="token punctuation">,</span><span class="token punctuation">[</span><span class="token number">56</span><span class="token punctuation">,</span><span class="token number">67</span><span class="token punctuation">,</span><span class="token number">78</span><span class="token punctuation">]</span><span class="token punctuation">}</span>

c <span class="token operator">=</span>

  <span class="token number">1</span>×<span class="token number">2</span> cell array

    <span class="token punctuation">{</span><span class="token string">'2017-08-16'</span><span class="token punctuation">}</span>    <span class="token punctuation">{</span><span class="token punctuation">[</span><span class="token number">56</span> <span class="token number">67</span> <span class="token number">78</span><span class="token punctuation">]</span><span class="token punctuation">}</span>
<span class="token comment">% Extracting 67</span>
<span class="token operator">&gt;</span><span class="token operator">&gt;</span> c<span class="token punctuation">{</span><span class="token number">2</span><span class="token punctuation">}</span><span class="token punctuation">(</span><span class="token number">2</span><span class="token punctuation">)</span>

ans <span class="token operator">=</span>

    <span class="token number">67</span>

</code></pre>
<h2 id="table-array">Table Array</h2>
<pre class=" language-matlab"><code class="prism  language-matlab">clc<span class="token punctuation">;</span>clear all<span class="token punctuation">;</span>

LastName <span class="token operator">=</span> <span class="token punctuation">{</span><span class="token string">'Sanchez'</span><span class="token punctuation">;</span><span class="token string">'Johnson'</span><span class="token punctuation">;</span><span class="token string">'Li'</span><span class="token punctuation">;</span><span class="token string">'Diaz'</span><span class="token punctuation">;</span><span class="token string">'Brown'</span><span class="token punctuation">}</span><span class="token punctuation">;</span>

Age <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">38</span><span class="token punctuation">;</span><span class="token number">43</span><span class="token punctuation">;</span><span class="token number">38</span><span class="token punctuation">;</span><span class="token number">40</span><span class="token punctuation">;</span><span class="token number">49</span><span class="token punctuation">]</span><span class="token punctuation">;</span>

Employed <span class="token operator">=</span> <span class="token function">logical</span><span class="token punctuation">(</span><span class="token punctuation">[</span><span class="token number">1</span><span class="token punctuation">;</span><span class="token number">0</span><span class="token punctuation">;</span><span class="token number">1</span><span class="token punctuation">;</span><span class="token number">0</span><span class="token punctuation">;</span><span class="token number">1</span><span class="token punctuation">]</span><span class="token punctuation">)</span><span class="token punctuation">;</span>

Height <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">71</span><span class="token punctuation">;</span><span class="token number">69</span><span class="token punctuation">;</span><span class="token number">64</span><span class="token punctuation">;</span><span class="token number">67</span><span class="token punctuation">;</span><span class="token number">64</span><span class="token punctuation">]</span><span class="token punctuation">;</span>

Weight <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">176</span><span class="token punctuation">;</span><span class="token number">163</span><span class="token punctuation">;</span><span class="token number">131</span><span class="token punctuation">;</span><span class="token number">133</span><span class="token punctuation">;</span><span class="token number">119</span><span class="token punctuation">]</span><span class="token punctuation">;</span>

BloodPressure <span class="token operator">=</span> <span class="token punctuation">[</span><span class="token number">124</span> <span class="token number">93</span><span class="token punctuation">;</span> <span class="token number">109</span> <span class="token number">77</span><span class="token punctuation">;</span> <span class="token number">125</span> <span class="token number">83</span><span class="token punctuation">;</span> <span class="token number">117</span> <span class="token number">75</span><span class="token punctuation">;</span> <span class="token number">122</span> <span class="token number">80</span><span class="token punctuation">]</span><span class="token punctuation">;</span>

T <span class="token operator">=</span> <span class="token function">table</span><span class="token punctuation">(</span>LastName<span class="token punctuation">,</span>Age<span class="token punctuation">,</span>Employed<span class="token punctuation">,</span>Height<span class="token punctuation">,</span>Weight<span class="token punctuation">,</span>BloodPressure<span class="token punctuation">)</span><span class="token punctuation">;</span>

City <span class="token operator">=</span> <span class="token punctuation">{</span><span class="token string">'Manipal'</span><span class="token punctuation">;</span><span class="token string">'Mumbai'</span><span class="token punctuation">;</span><span class="token string">'Pune'</span><span class="token punctuation">;</span><span class="token string">'Bangalore'</span><span class="token punctuation">;</span><span class="token string">'Delhi'</span><span class="token punctuation">}</span><span class="token punctuation">;</span>

T<span class="token punctuation">.</span>City <span class="token operator">=</span> City<span class="token punctuation">;</span>

T <span class="token operator">=</span>

  <span class="token number">5</span>×<span class="token number">7</span> table

     LastName      Age    Employed    Height    Weight    BloodPressure        City     
    ___________    ___    ________    ______    ______    _____________    _____________

    <span class="token punctuation">{</span><span class="token string">'Sanchez'</span><span class="token punctuation">}</span>    <span class="token number">38</span>      true         <span class="token number">71</span>       <span class="token number">176</span>       <span class="token number">124</span>     <span class="token number">93</span>      <span class="token punctuation">{</span><span class="token string">'Manipal'</span>  <span class="token punctuation">}</span>
    <span class="token punctuation">{</span><span class="token string">'Johnson'</span><span class="token punctuation">}</span>    <span class="token number">43</span>      false        <span class="token number">69</span>       <span class="token number">163</span>       <span class="token number">109</span>     <span class="token number">77</span>      <span class="token punctuation">{</span><span class="token string">'Mumbai'</span>   <span class="token punctuation">}</span>
    <span class="token punctuation">{</span><span class="token string">'Li'</span>     <span class="token punctuation">}</span>    <span class="token number">38</span>      true         <span class="token number">64</span>       <span class="token number">131</span>       <span class="token number">125</span>     <span class="token number">83</span>      <span class="token punctuation">{</span><span class="token string">'Pune'</span>     <span class="token punctuation">}</span>
    <span class="token punctuation">{</span><span class="token string">'Diaz'</span>   <span class="token punctuation">}</span>    <span class="token number">40</span>      false        <span class="token number">67</span>       <span class="token number">133</span>       <span class="token number">117</span>     <span class="token number">75</span>      <span class="token punctuation">{</span><span class="token string">'Bangalore'</span><span class="token punctuation">}</span>
    <span class="token punctuation">{</span><span class="token string">'Brown'</span>  <span class="token punctuation">}</span>    <span class="token number">49</span>      true         <span class="token number">64</span>       <span class="token number">119</span>       <span class="token number">122</span>     <span class="token number">80</span>      <span class="token punctuation">{</span><span class="token string">'Delhi'</span>    <span class="token punctuation">}</span>

<span class="token operator">&gt;</span><span class="token operator">&gt;</span>  maxHeight <span class="token operator">=</span> <span class="token function">max</span><span class="token punctuation">(</span>T<span class="token punctuation">.</span>Height<span class="token punctuation">)</span>

maxHeight <span class="token operator">=</span>

    <span class="token number">71</span>

T<span class="token punctuation">.</span>BMI <span class="token operator">=</span> <span class="token punctuation">(</span>T<span class="token punctuation">.</span>Weight<span class="token operator">*</span><span class="token number">0.453592</span><span class="token punctuation">)</span><span class="token operator">./</span><span class="token punctuation">(</span>T<span class="token punctuation">.</span>Height<span class="token operator">*</span><span class="token number">0.0254</span><span class="token punctuation">)</span><span class="token operator">.^</span><span class="token number">2</span><span class="token punctuation">;</span>


  <span class="token number">5</span>×<span class="token number">8</span> table

     LastName      Age    Employed    Height    Weight    BloodPressure        City          BMI  
    ___________    ___    ________    ______    ______    _____________    _____________    ______

    <span class="token punctuation">{</span><span class="token string">'Sanchez'</span><span class="token punctuation">}</span>    <span class="token number">38</span>      true         <span class="token number">71</span>       <span class="token number">176</span>       <span class="token number">124</span>     <span class="token number">93</span>      <span class="token punctuation">{</span><span class="token string">'Manipal'</span>  <span class="token punctuation">}</span>    <span class="token number">24.547</span>
    <span class="token punctuation">{</span><span class="token string">'Johnson'</span><span class="token punctuation">}</span>    <span class="token number">43</span>      false        <span class="token number">69</span>       <span class="token number">163</span>       <span class="token number">109</span>     <span class="token number">77</span>      <span class="token punctuation">{</span><span class="token string">'Mumbai'</span>   <span class="token punctuation">}</span>    <span class="token number">24.071</span>
    <span class="token punctuation">{</span><span class="token string">'Li'</span>     <span class="token punctuation">}</span>    <span class="token number">38</span>      true         <span class="token number">64</span>       <span class="token number">131</span>       <span class="token number">125</span>     <span class="token number">83</span>      <span class="token punctuation">{</span><span class="token string">'Pune'</span>     <span class="token punctuation">}</span>    <span class="token number">22.486</span>
    <span class="token punctuation">{</span><span class="token string">'Diaz'</span>   <span class="token punctuation">}</span>    <span class="token number">40</span>      false        <span class="token number">67</span>       <span class="token number">133</span>       <span class="token number">117</span>     <span class="token number">75</span>      <span class="token punctuation">{</span><span class="token string">'Bangalore'</span><span class="token punctuation">}</span>    <span class="token number">20.831</span>
    <span class="token punctuation">{</span><span class="token string">'Brown'</span>  <span class="token punctuation">}</span>    <span class="token number">49</span>      true         <span class="token number">64</span>       <span class="token number">119</span>       <span class="token number">122</span>     <span class="token number">80</span>      <span class="token punctuation">{</span><span class="token string">'Delhi'</span>    <span class="token punctuation">}</span>    <span class="token number">20.426</span>

</code></pre>

