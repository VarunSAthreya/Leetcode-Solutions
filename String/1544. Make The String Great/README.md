# [1544. Make The String Great](https://leetcode.com/problems/make-the-string-great/)

**Level:** `Easy`.

**Topic:** `String`, `Stack`.

Given a string <code>s</code> of lower and upper case English letters.

A good string is a string which doesn't have <strong>two adjacent characters</strong> <code>s[i]</code> and <code>s[i + 1]</code> where:

<ul>
 <li><code>0 &lt;= i &lt;= s.length - 2</code></li>
 <li><code>s[i]</code> is a lower-case letter and <code>s[i + 1]</code> is the same letter but in upper-case or <strong>vice-versa</strong>.</li>
</ul>

To make the string good, you can choose <strong>two adjacent</strong> characters that make the string bad and remove them. You can keep doing this until the string becomes good.

Return <em>the string</em> after making it good. The answer is guaranteed to be unique under the given constraints.

<strong>Notice</strong> that an empty string is also good.

<strong>Example 1:</strong>

<pre><strong>Input:</strong> s = "leEeetcode"
<strong>Output:</strong> "leetcode"
<strong>Explanation:</strong> In the first step, either you choose i = 1 or i = 2, both will result "leEeetcode" to be reduced to "leetcode".
</pre>

<strong>Example 2:</strong>

<pre><strong>Input:</strong> s = "abBAcC"
<strong>Output:</strong> ""
<strong>Explanation:</strong> We have many possible scenarios, and all lead to the same answer. For example:
"abBAcC" --&gt; "aAcC" --&gt; "cC" --&gt; ""
"abBAcC" --&gt; "abBA" --&gt; "aA" --&gt; ""
</pre>

<strong>Example 3:</strong>

<pre><strong>Input:</strong> s = "s"
<strong>Output:</strong> "s"
</pre>

<strong>Constraints:</strong>

<ul>
 <li><code>1 &lt;= s.length &lt;= 100</code></li>
 <li><code>s</code> contains only lower and upper case English letters.</li>
</ul>