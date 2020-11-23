<p> Assignment 6 <br>
Due: December 4, 2020 <br>

</p><ol class="enumerate" type=1><li class="li-enumerate">A <em>word ladder</em> is a sequence of English words connecting two given
English words such that consecutive words in the sequence differ by only one
letter. An example word ladder connecting FOOL and SAGE is
<pre class="verbatim">FOOL
POOL
POLL
POLE
PALE
SALE
SAGE
</pre>
There are many variations on the theme. One may be required to use a given
number of words, to use only words of a given length (or not), to use the
smallest numbers of words, etc.<ol class="enumerate" type=a><li class="li-enumerate">Using GiMPy, implement an algorithm for finding the shortest possible
word ladder connecting two given words of the same length. You might find
<div class="center">
<span style="font-family:monospace">https://github.com/dwyl/english-words</span>
</div>
useful.</li><li class="li-enumerate">By generating random pairs of words, determine (i) a lower bound on the
maximum size and (2) an estimate of the average size of a word ladder for
words of different lengths. Can you find a pair of words of the same length
for which there doesn&#X2019;t exist a word ladder? If running time is too long,
you may limit your dictionary in some reasonable way, but only if absolutely
necessary!</li><li class="li-enumerate">Make a graph of the length of time it takes to find a shortest word
ladder as a function of the length of the ladder.</li><li class="li-enumerate">Modify your algorithm to produce a word letter of a specified fixed
length if one exists.</li></ol></li><li class="li-enumerate">A <span style="font-style:italic">d</span>-heap is a heap in which non-leaf nodes in the tree can
have up to <span style="font-style:italic">d</span> children instead of just 2. <ol class="enumerate" type=a><li class="li-enumerate">Explain how to store a <span style="font-style:italic">d</span>-heap in an array.</li><li class="li-enumerate">What is the minimum height of a <span style="font-style:italic">d</span> heap of <span style="font-style:italic">n</span> elements in
terms of <span style="font-style:italic">n</span> and <span style="font-style:italic">d</span>?</li><li class="li-enumerate">Analyze the running times of the basic heap operations in terms
of <span style="font-style:italic">n</span> and <span style="font-style:italic">d</span>.</li></ol></li><li class="li-enumerate">Argue that the average depth of the tree in binary search is &#X398;(lg
<span style="font-style:italic">n</span>). Hint: write a recursion for the average depth a tree of size <span style="font-style:italic">n</span> and
solve it.</li><li class="li-enumerate">Suppose a list <span style="font-style:italic">A</span> contains only integers from 0 to 2<sup><span style="font-style:italic">i</span></sup> for some
given positive integer <span style="font-style:italic">i</span>. Explain how to do bissection search to find out
if a given integer appears in the list using only bit operations. This
method would be useful when <span style="font-style:italic">i</span> is very large and we cannot assume that the
basic operations involving the numbers in the array are constant-time. In
this case, the only operation we can use to access information about the
numbers in the array in constant-time is &#X201C;fetch the <span style="font-style:italic">j</span><sup>th</sup> bit
of <span style="font-style:italic">A</span>[<span style="font-style:italic">i</span>],&#X201D; which takes constant time. What is the running time of your
binary search algorithm in terms of the number of such operations? Your
running time may depend on what you assume about the input, such as whether
it is sorted and whether there are duplicates. For full credit, give the
running time with and without assumptions.</li><li class="li-enumerate">Suppose we have a graph with <span style="font-style:italic">n</span> vertices that is represented by
a set of <span style="font-style:italic">n</span> bit vectors <span style="font-style:italic">v</span><sup><span style="font-style:italic">i</span></sup>, where <span style="font-style:italic">v</span><sub><span style="font-style:italic">j</span></sub><sup><span style="font-style:italic">i</span></sup> = 1 if there is an
edge from vertex <span style="font-style:italic">i</span> to vertex <span style="font-style:italic">j</span>. Find an <span style="font-style:italic">O</span>(<span style="font-style:italic">n</span>) algorithm to
determine the vector <span style="font-style:italic">p</span><sup>1</sup> for which <span style="font-style:italic">p</span><sub><span style="font-style:italic">j</span></sub><sup>1</sup> = 1 if there is a path
from vertex 1 to vertex <span style="font-style:italic">j</span>. The operations you may use are
bitwise logical operations on bit vectors, arithmetic operations on
integers, instructions that set the value of a particular bit of a
particular vector, and an instruction that assigns the value <span style="font-style:italic">j</span> to
an integer variable <span style="font-style:italic">a</span> if the left-most &#X201C;1&#X201D; in a vector <span style="font-style:italic">v</span> is in
position <span style="font-style:italic">j</span> or sets <span style="font-style:italic">a</span> = 0 if <span style="font-style:italic">v</span> consists of all zeros. </li></ol>
