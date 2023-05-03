Download Link: https://assignmentchef.com/product/solved-cs2211a-assignment-5
<br>
A <em>complex number</em> is a number that can be expressed in the form <em>a + i b</em>, where <em>a</em> and <em>b</em> are real numbers and <em>i</em> is the imaginary unit, which satisfies the equation <em>i<sup>2</sup> = −1</em>.

In <em>a + i b</em>,  <em>a</em> is called the <em>real part</em> and <em>b</em> is called the <em>imaginary part</em> of the <em>complex number</em>.




Complex numbers extend the concept of the one-dimensional number line to the two-dimensional complex plane by using the horizontal axis for the real part and the vertical axis for the imaginary part.




<ol>

 <li><strong>(2 marks)</strong> Declare a tag named complex_tag for a structure with two members, real and imaginary, of type double.</li>

 <li><strong>(2 marks)</strong> Define a type (using typedef) named Complex_type for a structure with two members, real and imaginary, of type double.</li>

 <li><strong>(10 marks)</strong> Write a function that accepts two parameters of type complex_tag and returns a Complex_type of their multiplication.</li>

</ol>




Note that: if c<sub>1 </sub>and c<sub>2</sub> are two complex numbers, where c<sub>1</sub> = <em>a<sub>1</sub> + i b<sub>1</sub></em> and  c<sub>2</sub> = <em>a<sub>2</sub> + i b<sub>2</sub></em>, then <em>c<sub>1 </sub>× c<sub>2</sub> = (a<sub>1</sub> × a<sub>2 </sub>− b<sub>1</sub>× b<sub>2</sub>) + i (a<sub>2</sub> × b<sub>1 </sub>+ a<sub>1</sub> × b<sub>2</sub>)</em>

<ol>

 <li><strong>(15 marks)</strong> Write a function that accepts three parameters of type <strong><u>pointer</u></strong> to complex_tag and returns an <strong><em>integer</em></strong>. The function will set the content of the third complex_tag pointer to be the division result of the content of the first two complex_tag <strong><u>pointers</u></strong>.</li>

</ol>




Note that: if c<sub>1 </sub>and c<sub>2</sub> are two complex numbers, where c<sub>1</sub> = <em>a<sub>1</sub> + i b<sub>1</sub></em> and  c<sub>2</sub> = <em>a<sub>2</sub> + i b<sub>2</sub></em>, then

<em>c<sub>1 </sub>÷ c<sub>2</sub> = (a<sub>1</sub> × a<sub>2 </sub>+ b<sub>1</sub>× b<sub>2</sub>) ÷ (a<sub>2</sub><sup>2</sup> + b<sub>2</sub><sup>2</sup>) + i (a<sub>2</sub> × b<sub>1 </sub>− a<sub>1</sub> × b<sub>2</sub>) ÷ (a<sub>2</sub><sup>2</sup> + b</em><em> <strong> 0  </strong></em>

Note that, if <strong><em><u>(a<sub>2</sub></u><sup>2</sup><u> + b<sub>2</sub></u><sup>2</sup><u>) = 0</u></em></strong>, return -2, otherwise return 0.

<ol>

 <li><strong>(20 marks)</strong> Write a function that accepts four parameters: two parameters of type complex_tag and the other two of type <strong><u>pointer to a pointer</u></strong> to complex_tag. The function returns an <strong><em>integer</em></strong>. The function <strong><em>allocates</em></strong> memory for two complex_tag variables using the malloc Make sure that the <em>memory allocation operation</em> is successful before using its output Otherwise, you need to print an error message and return -1. The value of one of these two allocated complex_tag variables will be the sum of the first two arguments, while the other will be the difference between them. A pointer to one of these two created structures will be returned to the caller via the third parameter, while the pointer to the other created structure will be returned to the caller via the fourth parameter. Upon successfully calculating the sum and difference, return 0.</li>

</ol>




Note that: if c<sub>1 </sub>and c<sub>2</sub> are two complex numbers, where c<sub>1</sub> = <em>a<sub>1</sub> + i b<sub>1</sub></em> and  c<sub>2</sub> = <em>a<sub>2</sub> + i b<sub>2</sub></em>, then <em>c<sub>1 </sub><strong>+</strong> c<sub>2</sub> = (a<sub>1</sub> <strong>+</strong> a<sub>2</sub>) + i (b<sub>1 </sub><strong>+</strong> b<sub>2</sub>) c<sub>1</sub>  ̶  c<sub>2</sub> = (a<sub>1</sub>  ̶  a<sub>2</sub>) + i (b<sub>1</sub>    b̶ <sub>2</sub>)</em>

<ol>

 <li><strong>(4 marks)</strong> Put the three functions in a file called c and their prototypes in a file called operation_functions.h.</li>

 <li>Write a main program (c) that

  <ul>

   <li><strong>(10 marks)</strong> Declares two variables of type complex_tag. The value of these two variables will be initialized using the command-line arguments as 4 separate values, two for each variable.</li>

   <li><strong>(15 marks)</strong> Passes these initialized two structure variables (or a pointer to them, whenever appropriate) and whatever other arguments as needed to the three functions described above. Store the results in appropriate variables that you will also need to declare in the main function.</li>

   <li><strong>(5 marks)</strong> Prints the entered complex numbers, as well as the results of multiplication, division, addition, and subtraction operations in an easy-to-ready format.</li>

  </ul></li>

 <li><strong>(8 marks)</strong> Write an appropriate <strong><em>makefile</em></strong> that <strong><em>compiles</em></strong> and <strong><em>tests</em></strong> your program.</li>

 <li><strong>(2 marks)</strong> Provide a readme file that will tell how to use the make file to compile and/or test your program.</li>

</ol>




<ol>

 <li><strong>(7 marks)</strong> You should include as many test cases as possible to demonstrate various cases, e.g., dealing with

  <ul>

   <li>two complex numbers,</li>

   <li>two real numbers,</li>

   <li>two imaginary numbers,</li>

   <li>a real number and an imaginary number, P an imaginary number and a real number,</li>

   <li>a zero and a complex number, and</li>

   <li>a complex number and a zero.</li>

  </ul></li>

</ol>


