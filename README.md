# cmsc330-project-2-solved
**TO GET THIS SOLUTION VISIT:** [CMSC330 Project 2 Solved](https://www.ankitcodinghub.com/product/cmsc330-project-2-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;114874&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CMSC330 Project 2 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
The second project involves completing and extending the C++ program that evaluates statements of an expression language contained in the module 3 case study in the week 5 module reading.

The skeleton code for this project is attached. It differs slightly from the what is provided in the case study. The code in the case study allows only one expression to be input from the keyboard whereas the code in the attached skeleton accepts input from a file named <sub>input.txt</sub>. That file contains one statement per line.

The statements of that expression language consist of an arithmetic expression followed by a list of assignments. Assignments are separated from the expression and each other by commas. A semicolon terminates the expression. The arithmetic expressions are fully parenthesized infix expressions containing integer literals and variables. The syntax of a single input file line is described grammar below:

statement → expression ‘,’ assignments ‘;’ expression → ‘(‘&nbsp; operand operator operand ‘)’&nbsp;&nbsp; operator → ‘+’ | ‘-‘ operand → literal | variable | expression&nbsp; assignments → assignments ‘,’ assignment | assignment assignment → variable ‘=’ literal

In the above grammar, terminal symbols are upper case names or character literals shown in blue and nonterminal symbols are lower case names shown in red. EBNF metacharacters are shown in black. Tokens can be separated by any number of spaces.

Tokens can be separated by any number of spaces. Variable names begin with an alphabetic character, followed by any number of alphanumeric characters. Variable names are case sensitive. The regular expressions defining the variables and literal tokens are the following:

variable [a-zA-Z][a-zA-Z0-9]* literal [0-9]+

The program reads in the arithmetic expression and encodes the expression as a binary tree. After the expression has been read in, the variable assignments are read in and the variables and their values of the variables are placed into the symbol table. Finally the expression is evaluated recursively.

Your first task is to modify the program so that it will parse additional types of expressions defined by the expanded grammar shown below with the additions to the grammar highlighted in yellow:

statement → expression ‘,’ assignments ‘;’

expression → ‘(‘&nbsp; expressions ‘)’

<table width="599">
<tbody>
<tr>
<td colspan="2" width="599">expressions → unary_expression | binary_expression | ternary_expression |</td>
</tr>
<tr>
<td width="271">&nbsp; quaternary_expression | operand</td>
<td width="328"></td>
</tr>
</tbody>
</table>
unary_expression → expression ‘~’ binary_expression &nbsp;→ expression binary_operator expression binary_operator → ‘+’ | ‘-‘ | ‘*’ | ‘/’ | ‘%’ | ‘^’ | ‘&lt;‘ | ‘&gt;’ | ‘&amp;’ ternary_expression → expression ‘?’ expression expression quaternary_expression → expression ‘#’ expression expression expression operand → literal | variable | expression assignments → assignments ‘,’ assignment | assignment assignment → variable ‘=’ literal

The semantics of the additional binary arithmetic operators are as follows:

* Multiplication

/ Division

% Remainder

^ Exponentiation

Although two of the three additional binary operators are customarily relational operators in most languages, that is not true in this language. The semantics of all three of those operators are as follows:

&lt; Minimum (Evaluates to the minimum of the left and right operand)

&gt; Maximum (Evaluates to the maximum of the left and right operand)

&amp; Average (Evaluates to the average of the left and right operand)

The single unary operator <sub>~</sub> is the negation operator. Unlike the unary minus in most languages, it is a postfix operator rather than a prefix one.

The single ternary operator <sub>?</sub> is the conditional expression operator. Unlike the conditional expression operator in C++ and Java, no colon separates the second and third operands. This expression is evaluated as follows. If the expression to the left of the operator <sub>?</sub> is not 0, the value of the expression is the value of the first expression after the operator <sub>?</sub>. If it is 0, the value of the expression is the value of the second expression after the operator <sub>?</sub>.

The single quaternary operator <sub>#</sub> is a variation of the typical conditional expression operator. Like the ternary conditional expression operator, the remaining three operands are delimited only by whitespace. This expression is evaluated as follows. If the expression to the left of the operator <sub>#</sub> is less than 0, the value of the expression is the value of the first expression after the operator <sub>#</sub>. If it is equal to 0, the value of the expression is the value of the second expression after the operator <sub>#</sub>. If it is greater than 0, the value of the expression is the value of the third expression after the operator <sub>#</sub>.

The second task is to modifier the variable token so that underscores are permitted in all but the first character and modify the literal token so that it accepts unsigned floating point literals. Assignments also should be modified to allow assignment to values that are should also floating point rather than just integers.

The final task is to make the following modifications:

<ul>
<li>The symbol table should be initialized before each statement is evaluated, so that variables that are reused do not contain the value from a previous statement</li>
<li>Statements containing uninitialized variables should be reported as an error</li>
<li>A variable initialized more than once in a statement should be reported as an error (Creating an exception class to accommodate this error and the previous one is the recommended approach)</li>
</ul>
You may assume that all input is syntactically correct. No checks for syntax errors is required.

Each new class must be in a separate <sub>.h</sub> and .<sub>cpp</sub> pair of files. If all the functions in a class are one line functions, they can be implemented inline in <sub>.h</sub> file and the .<sub>cpp</sub> file can be omitted.

The deliverables for this project include the following:

<ol>
<li>A <sub>.zip</sub> file containing all the source code correctly implementing all required functionality.</li>
<li>All the <sub>.h</sub> and .<sub>cpp</sub> files provided in the skeleton should included regardless of whether they required any changes</li>
<li>All new files must include a header with the student name, date, project and a description of what the file contains</li>
<li>All modified files must include a header with the same information 2. A Word or PDF file that contains the following:</li>
<li>A discussion of how you approached the project</li>
<li>A test plan that contains test cases that include all additional images and test any new functionality. For each test case, the output produced should be included.</li>
<li>A discussion of lessons learned from the project and any improvements that could be made</li>
</ol>
