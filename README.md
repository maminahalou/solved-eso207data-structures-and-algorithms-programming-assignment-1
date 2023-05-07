Download Link: https://assignmentchef.com/product/solved-eso207data-structures-and-algorithms-programming-assignment-1
<br>






The faraway mythical land of Artemis, inhabited by Dryads, is in the shape of a giant equilateral triangle directed ”upwards”. Dryads are isolationist creatures and they live alone in equilateral triangles. Dryads also have another amusing feature. After one year, every Dryad in Artemis replicates into 4 dryads and relocates to a smaller equilateral triangle directed either ”upwards” or ”downwards”. Each year, when a dryad divides into four smaller dryads: three smaller dryad shift to smaller triangles directed in the same direction as their parent dryad, and one small dryad shifts to a smaller triangle directed in the opposite direction. Then each year this process repeats. The figure below illustrates this process.

Figure 1: How Dryads form their localities each year

Help the original dryad find out how many smaller dryads have localities that point ”upwards” in <em>n </em>years. As the number can be quite large, you should print it modulo 1000000007(10<sup>9 </sup>+ 7).

<strong>Example :</strong>

Let <em>n </em>= 3. Output will be 10.

<strong>Explanation :</strong>

Artemis is the first equilateral triangle with 1 dryad. At n=2, it divides into 4 dryad with 3 having smaller localities pointing ”upwards” and 1 directed ”downwards”. At n=3, each of these 4 replicate, thus giving the answer.

<ul>

 <li>(10 points) Let <em>U</em>(<em>n</em>) and <em>D</em>(<em>n</em>) be the total possible localities directed ”upwards” and ”downwards” respectively. Give the recurrence relations for <em>U</em>(<em>n</em>) and <em>D</em>(<em>n</em>). <em>U</em>(1) = 1<em>,D</em>(1) = 0.</li>

 <li>(40 points) <strong>Using recursive method</strong>, write a program that output <em>U</em>(<em>n</em>)<em>,D</em>(<em>n</em>) for a given <em>n</em>. 1 ≤ <em>n </em>≤ 10<sup>15</sup></li>

 <li>(60 points) <strong>Using iterative method</strong>, write a program that output <em>U</em>(<em>n</em>)<em>,D</em>(<em>n</em>) for a given <em>n</em>.

  <ul>

   <li>≤ <em>n </em>≤ 10<sup>15</sup></li>

  </ul></li>

</ul>

<ul>

 <li><strong>Using matrix exponentiation method</strong>, write a program that output <em>U</em>(<em>n</em>) for a given <em>n</em>.

  <ul>

   <li>≤ <em>n </em>≤ 10<sup>15</sup></li>

  </ul></li>

 <li> Generate a graph (<strong>Input (n) vs. Time required (micro-seconds)</strong>) for each of the above methods. You can use the python script in the following link for graph generation : <a href="https://gist.github.com/akashks1998/283410b3f014d5fc68b4766e32b35552">https://gist.github.com/akashks1998/283410b3f014d5fc68b4766e32b35552</a></li>

</ul>

For measuring time you can use other library functions. Refer to <a href="https://www.geeksforgeeks.org/how-to-measure-time-taken-by-a-program-in-c/">https://www.geeksforgeeks. </a><a href="https://www.geeksforgeeks.org/how-to-measure-time-taken-by-a-program-in-c/">org/how-to-measure-time-taken-by-a-program-in-c/</a> for more details on measuring time in C.

<strong>Inputs (n values) for which you have to generate Input vs Time required graph. Scale of the required time should be in micro-seconds.</strong>

<ul>

 <li>Recursive method: <em>n </em>= 1<em>,</em>2<em>,</em>3<em>,….,</em></li>

 <li>Iterative method: <em>n </em>= 1<em>,</em>500<em>,</em>1000<em>,</em>1500<em>,….,</em></li>

 <li>Power method: <em>n </em>= 1<em>,</em>10<em>,</em>100<em>,</em>1000<em>,….,</em>10<sup>15</sup>. [Use logarithmic scale for representing <em>n </em>values on X-axis in power method, i.e, values in X-axis should be from 0<em>,</em>1<em>,</em>2<em>,….,</em>15]</li>

</ul>

For each input in recursive and iterative method, calculate <em>U</em>(<em>n</em>)<em>,D</em>(<em>n</em>) 10 times and take the average time for plotting the graph. For power method the run time is quite small and will vary. So, for each input in this method, calculate <em>U</em>(<em>n</em>) 1000 times before taking the average time for graph generation.


