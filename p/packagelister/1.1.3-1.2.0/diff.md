# Comparing `tmp/packagelister-1.1.3.tar.gz` & `tmp/packagelister-1.2.0.tar.gz`

## Comparing `packagelister-1.1.3.tar` & `packagelister-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 packagelister-1.1.3/CHANGELOG.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 packagelister-1.1.3/docs/index.html
--rw-r--r--   0        0        0    34190 2020-02-02 00:00:00.000000 packagelister-1.1.3/docs/packagelister.html
--rw-r--r--   0        0        0    21653 2020-02-02 00:00:00.000000 packagelister-1.1.3/docs/search.js
--rw-r--r--   0        0        0    69384 2020-02-02 00:00:00.000000 packagelister-1.1.3/docs/packagelister/packagelister.html
--rw-r--r--   0        0        0    68862 2020-02-02 00:00:00.000000 packagelister-1.1.3/docs/packagelister/packagelister_cli.html
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 packagelister-1.1.3/src/packagelister/__init__.py
--rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 packagelister-1.1.3/src/packagelister/packagelister.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 packagelister-1.1.3/src/packagelister/packagelister_cli.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 packagelister-1.1.3/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 packagelister-1.1.3/LICENSE.txt
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 packagelister-1.1.3/README.md
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 packagelister-1.1.3/pyproject.toml
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 packagelister-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 packagelister-1.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 packagelister-1.2.0/docs/index.html
+-rw-r--r--   0        0        0    34190 2020-02-02 00:00:00.000000 packagelister-1.2.0/docs/packagelister.html
+-rw-r--r--   0        0        0    21653 2020-02-02 00:00:00.000000 packagelister-1.2.0/docs/search.js
+-rw-r--r--   0        0        0    69384 2020-02-02 00:00:00.000000 packagelister-1.2.0/docs/packagelister/packagelister.html
+-rw-r--r--   0        0        0    74342 2020-02-02 00:00:00.000000 packagelister-1.2.0/docs/packagelister/packagelister_cli.html
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 packagelister-1.2.0/src/packagelister/__init__.py
+-rw-r--r--   0        0        0     2973 2020-02-02 00:00:00.000000 packagelister-1.2.0/src/packagelister/packagelister.py
+-rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 packagelister-1.2.0/src/packagelister/packagelister_cli.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 packagelister-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 packagelister-1.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 packagelister-1.2.0/README.md
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 packagelister-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 packagelister-1.2.0/PKG-INFO
```

### Comparing `packagelister-1.1.3/docs/packagelister.html` & `packagelister-1.2.0/docs/packagelister.html`

 * *Files identical despite different names*

### Comparing `packagelister-1.1.3/docs/search.js` & `packagelister-1.2.0/docs/search.js`

 * *Files identical despite different names*

### Comparing `packagelister-1.1.3/docs/packagelister/packagelister.html` & `packagelister-1.2.0/docs/packagelister/packagelister.html`

 * *Files identical despite different names*

### Comparing `packagelister-1.1.3/docs/packagelister/packagelister_cli.html` & `packagelister-1.2.0/docs/packagelister/packagelister_cli.html`

 * *Files 4% similar despite different names*

```diff
@@ -83,64 +83,77 @@
 </span><span id="L-27"><a href="#L-27"><span class="linenos">27</span></a>            <span class="s2">&quot;-g&quot;</span><span class="p">,</span>
 </span><span id="L-28"><a href="#L-28"><span class="linenos">28</span></a>            <span class="s2">&quot;--generate_requirements&quot;</span><span class="p">,</span>
 </span><span id="L-29"><a href="#L-29"><span class="linenos">29</span></a>            <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
 </span><span id="L-30"><a href="#L-30"><span class="linenos">30</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Generate a requirements.txt file in --project_path. &quot;&quot;&quot;</span><span class="p">,</span>
 </span><span id="L-31"><a href="#L-31"><span class="linenos">31</span></a>        <span class="p">)</span>
 </span><span id="L-32"><a href="#L-32"><span class="linenos">32</span></a>
 </span><span id="L-33"><a href="#L-33"><span class="linenos">33</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="L-34"><a href="#L-34"><span class="linenos">34</span></a>            <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
-</span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a>            <span class="s2">&quot;--include_builtins&quot;</span><span class="p">,</span>
-</span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a>            <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Include built in standard library modules. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="L-38"><a href="#L-38"><span class="linenos">38</span></a>        <span class="p">)</span>
-</span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a>
-</span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="L-41"><a href="#L-41"><span class="linenos">41</span></a>
-</span><span id="L-42"><a href="#L-42"><span class="linenos">42</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">:</span>
-</span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">Path</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="L-44"><a href="#L-44"><span class="linenos">44</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="L-45"><a href="#L-45"><span class="linenos">45</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">)</span>
-</span><span id="L-46"><a href="#L-46"><span class="linenos">46</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">is_absolute</span><span class="p">():</span>
-</span><span id="L-47"><a href="#L-47"><span class="linenos">47</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">absolute</span><span class="p">()</span>
-</span><span id="L-48"><a href="#L-48"><span class="linenos">48</span></a>
-</span><span id="L-49"><a href="#L-49"><span class="linenos">49</span></a>        <span class="k">return</span> <span class="n">args</span>
+</span><span id="L-34"><a href="#L-34"><span class="linenos">34</span></a>            <span class="s2">&quot;-v&quot;</span><span class="p">,</span>
+</span><span id="L-35"><a href="#L-35"><span class="linenos">35</span></a>            <span class="s2">&quot;--versions&quot;</span><span class="p">,</span>
+</span><span id="L-36"><a href="#L-36"><span class="linenos">36</span></a>            <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="L-37"><a href="#L-37"><span class="linenos">37</span></a>            <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="L-38"><a href="#L-38"><span class="linenos">38</span></a>            <span class="n">choices</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;==&quot;</span><span class="p">,</span> <span class="s2">&quot;&lt;&quot;</span><span class="p">,</span> <span class="s2">&quot;&lt;=&quot;</span><span class="p">,</span> <span class="s2">&quot;&gt;&quot;</span><span class="p">,</span> <span class="s2">&quot;&gt;=&quot;</span><span class="p">,</span> <span class="s2">&quot;~=&quot;</span><span class="p">],</span>
+</span><span id="L-39"><a href="#L-39"><span class="linenos">39</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; When generating a requirements.txt file,</span>
+</span><span id="L-40"><a href="#L-40"><span class="linenos">40</span></a><span class="s2">            include the versions of the packages using this</span>
+</span><span id="L-41"><a href="#L-41"><span class="linenos">41</span></a><span class="s2">            relation.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-42"><a href="#L-42"><span class="linenos">42</span></a>        <span class="p">)</span>
+</span><span id="L-43"><a href="#L-43"><span class="linenos">43</span></a>
+</span><span id="L-44"><a href="#L-44"><span class="linenos">44</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="L-45"><a href="#L-45"><span class="linenos">45</span></a>            <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
+</span><span id="L-46"><a href="#L-46"><span class="linenos">46</span></a>            <span class="s2">&quot;--include_builtins&quot;</span><span class="p">,</span>
+</span><span id="L-47"><a href="#L-47"><span class="linenos">47</span></a>            <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="L-48"><a href="#L-48"><span class="linenos">48</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Include built in standard library modules. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="L-49"><a href="#L-49"><span class="linenos">49</span></a>        <span class="p">)</span>
 </span><span id="L-50"><a href="#L-50"><span class="linenos">50</span></a>
-</span><span id="L-51"><a href="#L-51"><span class="linenos">51</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="L-52"><a href="#L-52"><span class="linenos">52</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">scan</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">include_builtins</span><span class="p">)</span>
-</span><span id="L-53"><a href="#L-53"><span class="linenos">53</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">generate_requirements</span><span class="p">:</span>
-</span><span id="L-54"><a href="#L-54"><span class="linenos">54</span></a>        <span class="n">req_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">/</span> <span class="s2">&quot;requirements.txt&quot;</span>
-</span><span id="L-55"><a href="#L-55"><span class="linenos">55</span></a>        <span class="n">req_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
-</span><span id="L-56"><a href="#L-56"><span class="linenos">56</span></a>            <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="L-57"><a href="#L-57"><span class="linenos">57</span></a>                <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">~=</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-58"><a href="#L-58"><span class="linenos">58</span></a>                <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
-</span><span id="L-59"><a href="#L-59"><span class="linenos">59</span></a>                <span class="k">else</span> <span class="n">package</span>
-</span><span id="L-60"><a href="#L-60"><span class="linenos">60</span></a>                <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
-</span><span id="L-61"><a href="#L-61"><span class="linenos">61</span></a>            <span class="p">)</span>
-</span><span id="L-62"><a href="#L-62"><span class="linenos">62</span></a>        <span class="p">)</span>
-</span><span id="L-63"><a href="#L-63"><span class="linenos">63</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">{</span>
-</span><span id="L-64"><a href="#L-64"><span class="linenos">64</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">==</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">:</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]</span>
-</span><span id="L-65"><a href="#L-65"><span class="linenos">65</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
-</span><span id="L-66"><a href="#L-66"><span class="linenos">66</span></a>    <span class="p">}</span>
-</span><span id="L-67"><a href="#L-67"><span class="linenos">67</span></a>
-</span><span id="L-68"><a href="#L-68"><span class="linenos">68</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">show_files</span><span class="p">:</span>
-</span><span id="L-69"><a href="#L-69"><span class="linenos">69</span></a>        <span class="n">longest_key</span> <span class="o">=</span> <span class="nb">max</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">package</span><span class="p">)</span> <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">)</span>
-</span><span id="L-70"><a href="#L-70"><span class="linenos">70</span></a>        <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="L-71"><a href="#L-71"><span class="linenos">71</span></a>            <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="p">(</span><span class="n">longest_key</span><span class="o">-</span><span class="nb">len</span><span class="p">(</span><span class="n">package</span><span class="p">)</span><span class="o">+</span><span class="mi">4</span><span class="p">)</span><span class="si">}{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">Path</span><span class="p">(</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">relative_to</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">))</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">])</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="L-72"><a href="#L-72"><span class="linenos">72</span></a>            <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
-</span><span id="L-73"><a href="#L-73"><span class="linenos">73</span></a>        <span class="p">]</span>
-</span><span id="L-74"><a href="#L-74"><span class="linenos">74</span></a>
-</span><span id="L-75"><a href="#L-75"><span class="linenos">75</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Packages used in </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">:&quot;</span><span class="p">)</span>
-</span><span id="L-76"><a href="#L-76"><span class="linenos">76</span></a>    <span class="nb">print</span><span class="p">(</span>
-</span><span id="L-77"><a href="#L-77"><span class="linenos">77</span></a>        <span class="o">*</span><span class="n">packages</span><span class="p">,</span>
-</span><span id="L-78"><a href="#L-78"><span class="linenos">78</span></a>        <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">,</span>
-</span><span id="L-79"><a href="#L-79"><span class="linenos">79</span></a>    <span class="p">)</span>
+</span><span id="L-51"><a href="#L-51"><span class="linenos">51</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="L-52"><a href="#L-52"><span class="linenos">52</span></a>
+</span><span id="L-53"><a href="#L-53"><span class="linenos">53</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">:</span>
+</span><span id="L-54"><a href="#L-54"><span class="linenos">54</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">Path</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="L-55"><a href="#L-55"><span class="linenos">55</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="L-56"><a href="#L-56"><span class="linenos">56</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">)</span>
+</span><span id="L-57"><a href="#L-57"><span class="linenos">57</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">is_absolute</span><span class="p">():</span>
+</span><span id="L-58"><a href="#L-58"><span class="linenos">58</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">absolute</span><span class="p">()</span>
+</span><span id="L-59"><a href="#L-59"><span class="linenos">59</span></a>
+</span><span id="L-60"><a href="#L-60"><span class="linenos">60</span></a>        <span class="k">return</span> <span class="n">args</span>
+</span><span id="L-61"><a href="#L-61"><span class="linenos">61</span></a>
+</span><span id="L-62"><a href="#L-62"><span class="linenos">62</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="L-63"><a href="#L-63"><span class="linenos">63</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">scan</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">include_builtins</span><span class="p">)</span>
+</span><span id="L-64"><a href="#L-64"><span class="linenos">64</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">generate_requirements</span><span class="p">:</span>
+</span><span id="L-65"><a href="#L-65"><span class="linenos">65</span></a>        <span class="n">req_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">/</span> <span class="s2">&quot;requirements.txt&quot;</span>
+</span><span id="L-66"><a href="#L-66"><span class="linenos">66</span></a>        <span class="n">req_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
+</span><span id="L-67"><a href="#L-67"><span class="linenos">67</span></a>            <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="L-68"><a href="#L-68"><span class="linenos">68</span></a>                <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}{</span><span class="n">args</span><span class="o">.</span><span class="n">versions</span><span class="si">}{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-69"><a href="#L-69"><span class="linenos">69</span></a>                <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">versions</span>
+</span><span id="L-70"><a href="#L-70"><span class="linenos">70</span></a>                <span class="k">else</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-71"><a href="#L-71"><span class="linenos">71</span></a>                <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
+</span><span id="L-72"><a href="#L-72"><span class="linenos">72</span></a>                <span class="k">else</span> <span class="n">package</span>
+</span><span id="L-73"><a href="#L-73"><span class="linenos">73</span></a>                <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
+</span><span id="L-74"><a href="#L-74"><span class="linenos">74</span></a>            <span class="p">)</span>
+</span><span id="L-75"><a href="#L-75"><span class="linenos">75</span></a>        <span class="p">)</span>
+</span><span id="L-76"><a href="#L-76"><span class="linenos">76</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">{</span>
+</span><span id="L-77"><a href="#L-77"><span class="linenos">77</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">==</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">:</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]</span>
+</span><span id="L-78"><a href="#L-78"><span class="linenos">78</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
+</span><span id="L-79"><a href="#L-79"><span class="linenos">79</span></a>    <span class="p">}</span>
 </span><span id="L-80"><a href="#L-80"><span class="linenos">80</span></a>
-</span><span id="L-81"><a href="#L-81"><span class="linenos">81</span></a>
-</span><span id="L-82"><a href="#L-82"><span class="linenos">82</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
-</span><span id="L-83"><a href="#L-83"><span class="linenos">83</span></a>    <span class="n">main</span><span class="p">()</span>
+</span><span id="L-81"><a href="#L-81"><span class="linenos">81</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">show_files</span><span class="p">:</span>
+</span><span id="L-82"><a href="#L-82"><span class="linenos">82</span></a>        <span class="n">longest_key</span> <span class="o">=</span> <span class="nb">max</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">package</span><span class="p">)</span> <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">)</span>
+</span><span id="L-83"><a href="#L-83"><span class="linenos">83</span></a>        <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="L-84"><a href="#L-84"><span class="linenos">84</span></a>            <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="p">(</span><span class="n">longest_key</span><span class="o">-</span><span class="nb">len</span><span class="p">(</span><span class="n">package</span><span class="p">)</span><span class="o">+</span><span class="mi">4</span><span class="p">)</span><span class="si">}{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">Path</span><span class="p">(</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">relative_to</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">))</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">])</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="L-85"><a href="#L-85"><span class="linenos">85</span></a>            <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
+</span><span id="L-86"><a href="#L-86"><span class="linenos">86</span></a>        <span class="p">]</span>
+</span><span id="L-87"><a href="#L-87"><span class="linenos">87</span></a>
+</span><span id="L-88"><a href="#L-88"><span class="linenos">88</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Packages used in </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">:&quot;</span><span class="p">)</span>
+</span><span id="L-89"><a href="#L-89"><span class="linenos">89</span></a>    <span class="nb">print</span><span class="p">(</span>
+</span><span id="L-90"><a href="#L-90"><span class="linenos">90</span></a>        <span class="o">*</span><span class="n">packages</span><span class="p">,</span>
+</span><span id="L-91"><a href="#L-91"><span class="linenos">91</span></a>        <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">,</span>
+</span><span id="L-92"><a href="#L-92"><span class="linenos">92</span></a>    <span class="p">)</span>
+</span><span id="L-93"><a href="#L-93"><span class="linenos">93</span></a>
+</span><span id="L-94"><a href="#L-94"><span class="linenos">94</span></a>
+</span><span id="L-95"><a href="#L-95"><span class="linenos">95</span></a><span class="k">if</span> <span class="vm">__name__</span> <span class="o">==</span> <span class="s2">&quot;__main__&quot;</span><span class="p">:</span>
+</span><span id="L-96"><a href="#L-96"><span class="linenos">96</span></a>    <span class="n">main</span><span class="p">()</span>
 </span></pre></div>
 
 
             </section>
                 <section id="main">
                             <input id="main-view-source" class="view-source-toggle-state" type="checkbox" aria-hidden="true" tabindex="-1">
 <div class="attr function">
@@ -175,60 +188,73 @@
 </span><span id="main-28"><a href="#main-28"><span class="linenos">28</span></a>            <span class="s2">&quot;-g&quot;</span><span class="p">,</span>
 </span><span id="main-29"><a href="#main-29"><span class="linenos">29</span></a>            <span class="s2">&quot;--generate_requirements&quot;</span><span class="p">,</span>
 </span><span id="main-30"><a href="#main-30"><span class="linenos">30</span></a>            <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
 </span><span id="main-31"><a href="#main-31"><span class="linenos">31</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Generate a requirements.txt file in --project_path. &quot;&quot;&quot;</span><span class="p">,</span>
 </span><span id="main-32"><a href="#main-32"><span class="linenos">32</span></a>        <span class="p">)</span>
 </span><span id="main-33"><a href="#main-33"><span class="linenos">33</span></a>
 </span><span id="main-34"><a href="#main-34"><span class="linenos">34</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
-</span><span id="main-35"><a href="#main-35"><span class="linenos">35</span></a>            <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
-</span><span id="main-36"><a href="#main-36"><span class="linenos">36</span></a>            <span class="s2">&quot;--include_builtins&quot;</span><span class="p">,</span>
-</span><span id="main-37"><a href="#main-37"><span class="linenos">37</span></a>            <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
-</span><span id="main-38"><a href="#main-38"><span class="linenos">38</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Include built in standard library modules. &quot;&quot;&quot;</span><span class="p">,</span>
-</span><span id="main-39"><a href="#main-39"><span class="linenos">39</span></a>        <span class="p">)</span>
-</span><span id="main-40"><a href="#main-40"><span class="linenos">40</span></a>
-</span><span id="main-41"><a href="#main-41"><span class="linenos">41</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
-</span><span id="main-42"><a href="#main-42"><span class="linenos">42</span></a>
-</span><span id="main-43"><a href="#main-43"><span class="linenos">43</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">:</span>
-</span><span id="main-44"><a href="#main-44"><span class="linenos">44</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">Path</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
-</span><span id="main-45"><a href="#main-45"><span class="linenos">45</span></a>        <span class="k">else</span><span class="p">:</span>
-</span><span id="main-46"><a href="#main-46"><span class="linenos">46</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">)</span>
-</span><span id="main-47"><a href="#main-47"><span class="linenos">47</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">is_absolute</span><span class="p">():</span>
-</span><span id="main-48"><a href="#main-48"><span class="linenos">48</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">absolute</span><span class="p">()</span>
-</span><span id="main-49"><a href="#main-49"><span class="linenos">49</span></a>
-</span><span id="main-50"><a href="#main-50"><span class="linenos">50</span></a>        <span class="k">return</span> <span class="n">args</span>
+</span><span id="main-35"><a href="#main-35"><span class="linenos">35</span></a>            <span class="s2">&quot;-v&quot;</span><span class="p">,</span>
+</span><span id="main-36"><a href="#main-36"><span class="linenos">36</span></a>            <span class="s2">&quot;--versions&quot;</span><span class="p">,</span>
+</span><span id="main-37"><a href="#main-37"><span class="linenos">37</span></a>            <span class="nb">type</span><span class="o">=</span><span class="nb">str</span><span class="p">,</span>
+</span><span id="main-38"><a href="#main-38"><span class="linenos">38</span></a>            <span class="n">default</span><span class="o">=</span><span class="kc">None</span><span class="p">,</span>
+</span><span id="main-39"><a href="#main-39"><span class="linenos">39</span></a>            <span class="n">choices</span><span class="o">=</span><span class="p">[</span><span class="s2">&quot;==&quot;</span><span class="p">,</span> <span class="s2">&quot;&lt;&quot;</span><span class="p">,</span> <span class="s2">&quot;&lt;=&quot;</span><span class="p">,</span> <span class="s2">&quot;&gt;&quot;</span><span class="p">,</span> <span class="s2">&quot;&gt;=&quot;</span><span class="p">,</span> <span class="s2">&quot;~=&quot;</span><span class="p">],</span>
+</span><span id="main-40"><a href="#main-40"><span class="linenos">40</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; When generating a requirements.txt file,</span>
+</span><span id="main-41"><a href="#main-41"><span class="linenos">41</span></a><span class="s2">            include the versions of the packages using this</span>
+</span><span id="main-42"><a href="#main-42"><span class="linenos">42</span></a><span class="s2">            relation.&quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="main-43"><a href="#main-43"><span class="linenos">43</span></a>        <span class="p">)</span>
+</span><span id="main-44"><a href="#main-44"><span class="linenos">44</span></a>
+</span><span id="main-45"><a href="#main-45"><span class="linenos">45</span></a>        <span class="n">parser</span><span class="o">.</span><span class="n">add_argument</span><span class="p">(</span>
+</span><span id="main-46"><a href="#main-46"><span class="linenos">46</span></a>            <span class="s2">&quot;-i&quot;</span><span class="p">,</span>
+</span><span id="main-47"><a href="#main-47"><span class="linenos">47</span></a>            <span class="s2">&quot;--include_builtins&quot;</span><span class="p">,</span>
+</span><span id="main-48"><a href="#main-48"><span class="linenos">48</span></a>            <span class="n">action</span><span class="o">=</span><span class="s2">&quot;store_true&quot;</span><span class="p">,</span>
+</span><span id="main-49"><a href="#main-49"><span class="linenos">49</span></a>            <span class="n">help</span><span class="o">=</span><span class="s2">&quot;&quot;&quot; Include built in standard library modules. &quot;&quot;&quot;</span><span class="p">,</span>
+</span><span id="main-50"><a href="#main-50"><span class="linenos">50</span></a>        <span class="p">)</span>
 </span><span id="main-51"><a href="#main-51"><span class="linenos">51</span></a>
-</span><span id="main-52"><a href="#main-52"><span class="linenos">52</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
-</span><span id="main-53"><a href="#main-53"><span class="linenos">53</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">scan</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">include_builtins</span><span class="p">)</span>
-</span><span id="main-54"><a href="#main-54"><span class="linenos">54</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">generate_requirements</span><span class="p">:</span>
-</span><span id="main-55"><a href="#main-55"><span class="linenos">55</span></a>        <span class="n">req_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">/</span> <span class="s2">&quot;requirements.txt&quot;</span>
-</span><span id="main-56"><a href="#main-56"><span class="linenos">56</span></a>        <span class="n">req_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
-</span><span id="main-57"><a href="#main-57"><span class="linenos">57</span></a>            <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
-</span><span id="main-58"><a href="#main-58"><span class="linenos">58</span></a>                <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">~=</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="main-59"><a href="#main-59"><span class="linenos">59</span></a>                <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
-</span><span id="main-60"><a href="#main-60"><span class="linenos">60</span></a>                <span class="k">else</span> <span class="n">package</span>
-</span><span id="main-61"><a href="#main-61"><span class="linenos">61</span></a>                <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
-</span><span id="main-62"><a href="#main-62"><span class="linenos">62</span></a>            <span class="p">)</span>
-</span><span id="main-63"><a href="#main-63"><span class="linenos">63</span></a>        <span class="p">)</span>
-</span><span id="main-64"><a href="#main-64"><span class="linenos">64</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">{</span>
-</span><span id="main-65"><a href="#main-65"><span class="linenos">65</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">==</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">:</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]</span>
-</span><span id="main-66"><a href="#main-66"><span class="linenos">66</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
-</span><span id="main-67"><a href="#main-67"><span class="linenos">67</span></a>    <span class="p">}</span>
-</span><span id="main-68"><a href="#main-68"><span class="linenos">68</span></a>
-</span><span id="main-69"><a href="#main-69"><span class="linenos">69</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">show_files</span><span class="p">:</span>
-</span><span id="main-70"><a href="#main-70"><span class="linenos">70</span></a>        <span class="n">longest_key</span> <span class="o">=</span> <span class="nb">max</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">package</span><span class="p">)</span> <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">)</span>
-</span><span id="main-71"><a href="#main-71"><span class="linenos">71</span></a>        <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
-</span><span id="main-72"><a href="#main-72"><span class="linenos">72</span></a>            <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="p">(</span><span class="n">longest_key</span><span class="o">-</span><span class="nb">len</span><span class="p">(</span><span class="n">package</span><span class="p">)</span><span class="o">+</span><span class="mi">4</span><span class="p">)</span><span class="si">}{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">Path</span><span class="p">(</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">relative_to</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">))</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">])</span><span class="si">}</span><span class="s2">&quot;</span>
-</span><span id="main-73"><a href="#main-73"><span class="linenos">73</span></a>            <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
-</span><span id="main-74"><a href="#main-74"><span class="linenos">74</span></a>        <span class="p">]</span>
-</span><span id="main-75"><a href="#main-75"><span class="linenos">75</span></a>
-</span><span id="main-76"><a href="#main-76"><span class="linenos">76</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Packages used in </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">:&quot;</span><span class="p">)</span>
-</span><span id="main-77"><a href="#main-77"><span class="linenos">77</span></a>    <span class="nb">print</span><span class="p">(</span>
-</span><span id="main-78"><a href="#main-78"><span class="linenos">78</span></a>        <span class="o">*</span><span class="n">packages</span><span class="p">,</span>
-</span><span id="main-79"><a href="#main-79"><span class="linenos">79</span></a>        <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">,</span>
-</span><span id="main-80"><a href="#main-80"><span class="linenos">80</span></a>    <span class="p">)</span>
+</span><span id="main-52"><a href="#main-52"><span class="linenos">52</span></a>        <span class="n">args</span> <span class="o">=</span> <span class="n">parser</span><span class="o">.</span><span class="n">parse_args</span><span class="p">()</span>
+</span><span id="main-53"><a href="#main-53"><span class="linenos">53</span></a>
+</span><span id="main-54"><a href="#main-54"><span class="linenos">54</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">:</span>
+</span><span id="main-55"><a href="#main-55"><span class="linenos">55</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">Path</span><span class="o">.</span><span class="n">cwd</span><span class="p">()</span>
+</span><span id="main-56"><a href="#main-56"><span class="linenos">56</span></a>        <span class="k">else</span><span class="p">:</span>
+</span><span id="main-57"><a href="#main-57"><span class="linenos">57</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">Path</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">)</span>
+</span><span id="main-58"><a href="#main-58"><span class="linenos">58</span></a>        <span class="k">if</span> <span class="ow">not</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">is_absolute</span><span class="p">():</span>
+</span><span id="main-59"><a href="#main-59"><span class="linenos">59</span></a>            <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">absolute</span><span class="p">()</span>
+</span><span id="main-60"><a href="#main-60"><span class="linenos">60</span></a>
+</span><span id="main-61"><a href="#main-61"><span class="linenos">61</span></a>        <span class="k">return</span> <span class="n">args</span>
+</span><span id="main-62"><a href="#main-62"><span class="linenos">62</span></a>
+</span><span id="main-63"><a href="#main-63"><span class="linenos">63</span></a>    <span class="n">args</span> <span class="o">=</span> <span class="n">get_args</span><span class="p">()</span>
+</span><span id="main-64"><a href="#main-64"><span class="linenos">64</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="n">scan</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">,</span> <span class="n">args</span><span class="o">.</span><span class="n">include_builtins</span><span class="p">)</span>
+</span><span id="main-65"><a href="#main-65"><span class="linenos">65</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">generate_requirements</span><span class="p">:</span>
+</span><span id="main-66"><a href="#main-66"><span class="linenos">66</span></a>        <span class="n">req_path</span> <span class="o">=</span> <span class="n">args</span><span class="o">.</span><span class="n">project_path</span> <span class="o">/</span> <span class="s2">&quot;requirements.txt&quot;</span>
+</span><span id="main-67"><a href="#main-67"><span class="linenos">67</span></a>        <span class="n">req_path</span><span class="o">.</span><span class="n">write_text</span><span class="p">(</span>
+</span><span id="main-68"><a href="#main-68"><span class="linenos">68</span></a>            <span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+</span><span id="main-69"><a href="#main-69"><span class="linenos">69</span></a>                <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}{</span><span class="n">args</span><span class="o">.</span><span class="n">versions</span><span class="si">}{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="main-70"><a href="#main-70"><span class="linenos">70</span></a>                <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">versions</span>
+</span><span id="main-71"><a href="#main-71"><span class="linenos">71</span></a>                <span class="k">else</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="main-72"><a href="#main-72"><span class="linenos">72</span></a>                <span class="k">if</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;version&quot;</span><span class="p">]</span>
+</span><span id="main-73"><a href="#main-73"><span class="linenos">73</span></a>                <span class="k">else</span> <span class="n">package</span>
+</span><span id="main-74"><a href="#main-74"><span class="linenos">74</span></a>                <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
+</span><span id="main-75"><a href="#main-75"><span class="linenos">75</span></a>            <span class="p">)</span>
+</span><span id="main-76"><a href="#main-76"><span class="linenos">76</span></a>        <span class="p">)</span>
+</span><span id="main-77"><a href="#main-77"><span class="linenos">77</span></a>    <span class="n">packages</span> <span class="o">=</span> <span class="p">{</span>
+</span><span id="main-78"><a href="#main-78"><span class="linenos">78</span></a>        <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}</span><span class="s2">==</span><span class="si">{</span><span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s1">&#39;version&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">&quot;</span><span class="p">:</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">][</span><span class="s2">&quot;files&quot;</span><span class="p">]</span>
+</span><span id="main-79"><a href="#main-79"><span class="linenos">79</span></a>        <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="nb">sorted</span><span class="p">(</span><span class="n">packages</span><span class="p">)</span>
+</span><span id="main-80"><a href="#main-80"><span class="linenos">80</span></a>    <span class="p">}</span>
+</span><span id="main-81"><a href="#main-81"><span class="linenos">81</span></a>
+</span><span id="main-82"><a href="#main-82"><span class="linenos">82</span></a>    <span class="k">if</span> <span class="n">args</span><span class="o">.</span><span class="n">show_files</span><span class="p">:</span>
+</span><span id="main-83"><a href="#main-83"><span class="linenos">83</span></a>        <span class="n">longest_key</span> <span class="o">=</span> <span class="nb">max</span><span class="p">(</span><span class="nb">len</span><span class="p">(</span><span class="n">package</span><span class="p">)</span> <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">)</span>
+</span><span id="main-84"><a href="#main-84"><span class="linenos">84</span></a>        <span class="n">packages</span> <span class="o">=</span> <span class="p">[</span>
+</span><span id="main-85"><a href="#main-85"><span class="linenos">85</span></a>            <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">package</span><span class="si">}{</span><span class="s1">&#39; &#39;</span><span class="o">*</span><span class="p">(</span><span class="n">longest_key</span><span class="o">-</span><span class="nb">len</span><span class="p">(</span><span class="n">package</span><span class="p">)</span><span class="o">+</span><span class="mi">4</span><span class="p">)</span><span class="si">}{</span><span class="s1">&#39;, &#39;</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="nb">str</span><span class="p">(</span><span class="n">Path</span><span class="p">(</span><span class="n">file</span><span class="p">)</span><span class="o">.</span><span class="n">relative_to</span><span class="p">(</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="p">))</span> <span class="k">for</span> <span class="n">file</span> <span class="ow">in</span> <span class="n">packages</span><span class="p">[</span><span class="n">package</span><span class="p">])</span><span class="si">}</span><span class="s2">&quot;</span>
+</span><span id="main-86"><a href="#main-86"><span class="linenos">86</span></a>            <span class="k">for</span> <span class="n">package</span> <span class="ow">in</span> <span class="n">packages</span>
+</span><span id="main-87"><a href="#main-87"><span class="linenos">87</span></a>        <span class="p">]</span>
+</span><span id="main-88"><a href="#main-88"><span class="linenos">88</span></a>
+</span><span id="main-89"><a href="#main-89"><span class="linenos">89</span></a>    <span class="nb">print</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Packages used in </span><span class="si">{</span><span class="n">args</span><span class="o">.</span><span class="n">project_path</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">:&quot;</span><span class="p">)</span>
+</span><span id="main-90"><a href="#main-90"><span class="linenos">90</span></a>    <span class="nb">print</span><span class="p">(</span>
+</span><span id="main-91"><a href="#main-91"><span class="linenos">91</span></a>        <span class="o">*</span><span class="n">packages</span><span class="p">,</span>
+</span><span id="main-92"><a href="#main-92"><span class="linenos">92</span></a>        <span class="n">sep</span><span class="o">=</span><span class="s2">&quot;</span><span class="se">\n</span><span class="s2">&quot;</span><span class="p">,</span>
+</span><span id="main-93"><a href="#main-93"><span class="linenos">93</span></a>    <span class="p">)</span>
 </span></pre></div>
 
 
     
 
                 </section>
     </main>
```

#### html2text {}

```diff
@@ -37,66 +37,79 @@
 27            "-g",
 28            "--generate_requirements",
 29            action="store_true",
 30            help=""" Generate a requirements.txt file in --project_path. """,
 31        )
 32
 33        parser.add_argument(
-34            "-i",
-35            "--include_builtins",
-36            action="store_true",
-37            help=""" Include built in standard library modules. """,
-38        )
-39
-40        args = parser.parse_args()
-41
-42        if not args.project_path:
-43            args.project_path = Path.cwd()
-44        else:
-45            args.project_path = Path(args.project_path)
-46        if not args.project_path.is_absolute():
-47            args.project_path = args.project_path.absolute()
-48
-49        return args
+34            "-v",
+35            "--versions",
+36            type=str,
+37            default=None,
+38            choices=["==", "<", "<=", ">", ">=", "~="],
+39            help=""" When generating a requirements.txt file,
+40            include the versions of the packages using this
+41            relation.""",
+42        )
+43
+44        parser.add_argument(
+45            "-i",
+46            "--include_builtins",
+47            action="store_true",
+48            help=""" Include built in standard library modules. """,
+49        )
 50
-51    args = get_args()
-52    packages = scan(args.project_path, args.include_builtins)
-53    if args.generate_requirements:
-54        req_path = args.project_path / "requirements.txt"
-55        req_path.write_text(
-56            "\n".join(
-57                f"{package}~={packages[package]['version']}"
-58                if packages[package]["version"]
-59                else package
-60                for package in sorted(packages)
-61            )
-62        )
-63    packages = {
-64        f"{package}=={packages[package]['version']}": packages[package]
+51        args = parser.parse_args()
+52
+53        if not args.project_path:
+54            args.project_path = Path.cwd()
+55        else:
+56            args.project_path = Path(args.project_path)
+57        if not args.project_path.is_absolute():
+58            args.project_path = args.project_path.absolute()
+59
+60        return args
+61
+62    args = get_args()
+63    packages = scan(args.project_path, args.include_builtins)
+64    if args.generate_requirements:
+65        req_path = args.project_path / "requirements.txt"
+66        req_path.write_text(
+67            "\n".join(
+68                f"{package}{args.versions}{packages[package]['version']}"
+69                if args.versions
+70                else f"{package}"
+71                if packages[package]["version"]
+72                else package
+73                for package in sorted(packages)
+74            )
+75        )
+76    packages = {
+77        f"{package}=={packages[package]['version']}": packages[package]
 ["files"]
-65        for package in sorted(packages)
-66    }
-67
-68    if args.show_files:
-69        longest_key = max(len(package) for package in packages)
-70        packages = [
-71            f"{package}{' '*(longest_key-len(package)+4)}{', '.join(str(Path
-(file).relative_to(args.project_path)) for file in packages[package])}"
-72            for package in packages
-73        ]
-74
-75    print(f"Packages used in {args.project_path.stem}:")
-76    print(
-77        *packages,
-78        sep="\n",
-79    )
+78        for package in sorted(packages)
+79    }
 80
-81
-82if __name__ == "__main__":
-83    main()
+81    if args.show_files:
+82        longest_key = max(len(package) for package in packages)
+83        packages = [
+84            f"{package}{' '*(longest_key-len(package)+4)}{', '.join(str(Path
+(file).relative_to(args.project_path)) for file in packages[package])}"
+85            for package in packages
+86        ]
+87
+88    print(f"Packages used in {args.project_path.stem}:")
+89    print(
+90        *packages,
+91        sep="\n",
+92    )
+93
+94
+95if __name__ == "__main__":
+96    main()
   ⁰
 def main(): View Source
 _8def main():
 _9    def get_args() -> argparse.Namespace:
 10        parser = argparse.ArgumentParser()
 11
 12        parser.add_argument(
@@ -118,56 +131,69 @@
 28            "-g",
 29            "--generate_requirements",
 30            action="store_true",
 31            help=""" Generate a requirements.txt file in --project_path. """,
 32        )
 33
 34        parser.add_argument(
-35            "-i",
-36            "--include_builtins",
-37            action="store_true",
-38            help=""" Include built in standard library modules. """,
-39        )
-40
-41        args = parser.parse_args()
-42
-43        if not args.project_path:
-44            args.project_path = Path.cwd()
-45        else:
-46            args.project_path = Path(args.project_path)
-47        if not args.project_path.is_absolute():
-48            args.project_path = args.project_path.absolute()
-49
-50        return args
+35            "-v",
+36            "--versions",
+37            type=str,
+38            default=None,
+39            choices=["==", "<", "<=", ">", ">=", "~="],
+40            help=""" When generating a requirements.txt file,
+41            include the versions of the packages using this
+42            relation.""",
+43        )
+44
+45        parser.add_argument(
+46            "-i",
+47            "--include_builtins",
+48            action="store_true",
+49            help=""" Include built in standard library modules. """,
+50        )
 51
-52    args = get_args()
-53    packages = scan(args.project_path, args.include_builtins)
-54    if args.generate_requirements:
-55        req_path = args.project_path / "requirements.txt"
-56        req_path.write_text(
-57            "\n".join(
-58                f"{package}~={packages[package]['version']}"
-59                if packages[package]["version"]
-60                else package
-61                for package in sorted(packages)
-62            )
-63        )
-64    packages = {
-65        f"{package}=={packages[package]['version']}": packages[package]
+52        args = parser.parse_args()
+53
+54        if not args.project_path:
+55            args.project_path = Path.cwd()
+56        else:
+57            args.project_path = Path(args.project_path)
+58        if not args.project_path.is_absolute():
+59            args.project_path = args.project_path.absolute()
+60
+61        return args
+62
+63    args = get_args()
+64    packages = scan(args.project_path, args.include_builtins)
+65    if args.generate_requirements:
+66        req_path = args.project_path / "requirements.txt"
+67        req_path.write_text(
+68            "\n".join(
+69                f"{package}{args.versions}{packages[package]['version']}"
+70                if args.versions
+71                else f"{package}"
+72                if packages[package]["version"]
+73                else package
+74                for package in sorted(packages)
+75            )
+76        )
+77    packages = {
+78        f"{package}=={packages[package]['version']}": packages[package]
 ["files"]
-66        for package in sorted(packages)
-67    }
-68
-69    if args.show_files:
-70        longest_key = max(len(package) for package in packages)
-71        packages = [
-72            f"{package}{' '*(longest_key-len(package)+4)}{', '.join(str(Path
+79        for package in sorted(packages)
+80    }
+81
+82    if args.show_files:
+83        longest_key = max(len(package) for package in packages)
+84        packages = [
+85            f"{package}{' '*(longest_key-len(package)+4)}{', '.join(str(Path
 (file).relative_to(args.project_path)) for file in packages[package])}"
-73            for package in packages
-74        ]
-75
-76    print(f"Packages used in {args.project_path.stem}:")
-77    print(
-78        *packages,
-79        sep="\n",
-80    )
+86            for package in packages
+87        ]
+88
+89    print(f"Packages used in {args.project_path.stem}:")
+90    print(
+91        *packages,
+92        sep="\n",
+93    )
```

### Comparing `packagelister-1.1.3/src/packagelister/packagelister.py` & `packagelister-1.2.0/src/packagelister/packagelister.py`

 * *Files identical despite different names*

### Comparing `packagelister-1.1.3/src/packagelister/packagelister_cli.py` & `packagelister-1.2.0/src/packagelister/packagelister_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,25 @@
             "-g",
             "--generate_requirements",
             action="store_true",
             help=""" Generate a requirements.txt file in --project_path. """,
         )
 
         parser.add_argument(
+            "-v",
+            "--versions",
+            type=str,
+            default=None,
+            choices=["==", "<", "<=", ">", ">=", "~="],
+            help=""" When generating a requirements.txt file,
+            include the versions of the packages using this
+            relation.""",
+        )
+
+        parser.add_argument(
             "-i",
             "--include_builtins",
             action="store_true",
             help=""" Include built in standard library modules. """,
         )
 
         args = parser.parse_args()
@@ -50,15 +61,17 @@
 
     args = get_args()
     packages = scan(args.project_path, args.include_builtins)
     if args.generate_requirements:
         req_path = args.project_path / "requirements.txt"
         req_path.write_text(
             "\n".join(
-                f"{package}~={packages[package]['version']}"
+                f"{package}{args.versions}{packages[package]['version']}"
+                if args.versions
+                else f"{package}"
                 if packages[package]["version"]
                 else package
                 for package in sorted(packages)
             )
         )
     packages = {
         f"{package}=={packages[package]['version']}": packages[package]["files"]
```

### Comparing `packagelister-1.1.3/LICENSE.txt` & `packagelister-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `packagelister-1.1.3/README.md` & `packagelister-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `packagelister-1.1.3/pyproject.toml` & `packagelister-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 00000070: 0d0a 6175 7468 6f72 7320 3d20 5b7b 6e61  ..authors = [{na
 00000080: 6d65 3d22 4d61 7474 204d 616e 6573 227d  me="Matt Manes"}
 00000090: 5d0d 0a64 6573 6372 6970 7469 6f6e 203d  ]..description =
 000000a0: 2022 4465 7465 726d 696e 6520 7768 6174   "Determine what
 000000b0: 2033 7264 2d70 6172 7479 2070 6163 6b61   3rd-party packa
 000000c0: 6765 7320 6120 7072 6f6a 6563 7420 696d  ges a project im
 000000d0: 706f 7274 732e 220d 0a76 6572 7369 6f6e  ports."..version
-000000e0: 203d 2022 312e 312e 3322 0d0a 7265 7175   = "1.1.3"..requ
+000000e0: 203d 2022 312e 322e 3022 0d0a 7265 7175   = "1.2.0"..requ
 000000f0: 6972 6573 2d70 7974 686f 6e20 3d20 223e  ires-python = ">
 00000100: 3d33 2e31 3022 0d0a 6465 7065 6e64 656e  =3.10"..dependen
 00000110: 6369 6573 203d 205b 2270 6174 6863 7261  cies = ["pathcra
 00000120: 776c 6572 222c 2022 7072 696e 7462 7564  wler", "printbud
 00000130: 6469 6573 222c 2022 7079 7465 7374 225d  dies", "pytest"]
 00000140: 0d0a 7265 6164 6d65 203d 2022 5245 4144  ..readme = "READ
 00000150: 4d45 2e6d 6422 0d0a 6b65 7977 6f72 6473  ME.md"..keywords
```

### Comparing `packagelister-1.1.3/PKG-INFO` & `packagelister-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packagelister
-Version: 1.1.3
+Version: 1.2.0
 Summary: Determine what 3rd-party packages a project imports.
 Project-URL: Homepage, https://github.com/matt-manes/packagelister
 Project-URL: Documentation, https://github.com/matt-manes/packagelister/tree/main/docs
 Project-URL: Source code, https://github.com/matt-manes/packagelister/tree/main/src/packagelister
 Author: Matt Manes
 License-File: LICENSE.txt
 Keywords: import,module,package
```

