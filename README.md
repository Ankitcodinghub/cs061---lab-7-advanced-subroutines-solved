# cs061---lab-7-advanced-subroutines-solved
**TO GET THIS SOLUTION VISIT:** [CS061 – Lab 7 Advanced subroutines! Solved](https://www.ankitcodinghub.com/product/cs061-lab-7-advanced-subroutines-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;99937&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS061 – Lab 7  Advanced subroutines! Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

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
<h1>1&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; High Level Description</h1>
The purpose of this lab is to teach you some advanced subroutine techniques that allow you to write recursive subroutines (a subroutine that calls itself directly or indirectly)!

<h1>2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Our Objectives for This Week</h1>
<ol>
<li>Exercise 1 ~ Demonstrate the shortcomings of subroutine protocols from the book</li>
<li>Exercise 2 ~ Improve upon the book’s subroutine protocols and show the shortcomings even with this improvement</li>
<li>Exercise 3 ~ Refine the subroutine protocols by using stacks to allow for recursion</li>
</ol>
<strong><u>3.1&nbsp;&nbsp; Exercises</u></strong>

<u>Exercise 1</u>

Recall that the definition of Factorial is 𝑛! &nbsp;× 𝑛 or as the computing the 𝑛<sup>th</sup>𝑛factorial relies on computing𝑛 − 1 × 𝑛 the (𝑛 − 1)<sup>th </sup>factorial.

relation Factorial( ) = Factorial(&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ) relation is defined as a recursive relation since

We can implement a recursive relation using a recursive subroutine. A recursive subroutine is any subroutine that calls itself either directly or indirectly. A directly recursive subroutine makes a direct call to itself within the subroutine. An indirectly recursive subroutine makes no direct call to itself, but rather calls another subroutine that calls itself. Either way, we need to write our subroutines carefully so that they support recursion, even if we did not deliberately write it to be recursive (in other words, indirectly recursive).

For this exercise, load the provided code from the lab7_ex1.asm file into the LC-3 tools program, assemble, and run the code in the simulator. What happens? (In order to recover from what happens, hit the pause button in the simulator)

<em>Ex 1. Q1. What happens when you run this code?</em>

Now reset the simulator so you can run the program again. This time, you will step through the code to discover why the program behaved the way it did. Remember, our eventual goal is to implement recursion and this program fails when returning from the original subroutine called after it stops recursing.

Put a breakpoint on address x3003. This should correspond to the instruction ‘JSRR R6’ which calls the first subroutine. Press play and wait for the program to stop at that breakpoint. Next press the ‘Step in’ icon. That’s the icon that looks like a right angle with an arrow pointing to the right. This action will step into the subroutine that is at the address in register R6, which should be x3200.

Next, put a breakpoint on address x3205. This should correspond to the instruction ‘JSR FACT_SUB_START’. Now note the values in R0 and R1.

<em>Ex 1. Q2. What are the values in registers R0 and R1?</em>

Press the play button one more time.

<em>Ex 1. Q3. What are the values in registers R0 and R1 after pressing play, but before pressing any other buttons?</em>

Then from there use the ‘Step in’ button. If you use the ‘Step over’ button you won’t be able to observe the recursion.

The register R1 will count down from 5 to 0 upon each invocation of the recursion. Once R0 has the value 0, it will stop recursing and finish executing the last call to the FACT subroutine. It stops because of the branch instruction in address x3204 which has the instruction ‘BRz BASE_3200’. The condition code is finally zero upon the last decrement of R1 in the previous address.

Ex 1. Q4 Write the values of registers R0 and R1 for each iteration of the recursion until the recursion stops. You’ll know the recursion stops when the program is on the instruction in address x320B, which corresponds to the BASE_3200 label.

<table width="232">
<tbody>
<tr>
<td width="120"><strong>R0</strong></td>
<td width="112"><strong>R1</strong></td>
</tr>
<tr>
<td width="120"></td>
<td width="112"></td>
</tr>
<tr>
<td width="120"></td>
<td width="112"></td>
</tr>
<tr>
<td width="120"></td>
<td width="112"></td>
</tr>
<tr>
<td width="120"></td>
<td width="112"></td>
</tr>
</tbody>
</table>
Now continue pressing the ‘Step in’ button until you reach address x3210 which has the instruction ‘RET’. The RET instruction is a pseudo-instruction for ‘JMP R7’. That means that it jumps to the instruction at the address in R7.

<em>EX 1. Q5. What is the value of R7 before you execute the RET instruction?</em>

Now press ‘Step in’ and you should go back to the address from your answer above and execution will continue executing from there.

<em>EX 1. Q6. What is the value of R7 every time you get to return after the first time? (Don’t worry if you miss it the first time, it will be the same forever)</em>

The program is now stuck in an infinite loop of returning to the address from Ex 1. Q 6. Above.

Discuss with the TA why that is and any possible solution to this problem. (Hint: Look at the next exercise)

<u>Exercise 2</u>

The shortcoming of the code in the previous exercise is that the R7 register was not backed up and restored in the subroutines like the other registers used. We learned in Lab 5 to always back up and restore R7.

For this exercise, copy your code from lab 7 exercise 1 above into the file lab7_ex2.asm. Then modify both the FACT and MUL subroutines to properly backup and restore the R7 register as we learned in lab 5. Once you’ve made this change, assemble and run the code.

<em>Ex 2. Q 1. What happens this time when you run the code?</em>

(You’ll need to press the pause button in the simulator again to recover from what happens)

Again, put a breakpoint on address x3003. This should correspond to the instruction ‘JSRR R6’ which calls the first subroutine. Press play and wait for the program to stop at that breakpoint. Next press the ‘Step in’ icon. That’s the icon that looks like a right angle with an arrow pointing to the right. This action will step into the subroutine that is at the address in register R6, which should be x3200.

This time, put a breakpoint on the line corresponding to ‘JSR FACT_SUB_START’ (it will have moved after adding lines to backup/restore R7). Now note the values in R0 and R1.

<em>Ex 2. Q2. What are the values in registers R0 and R1?</em>

Press the play button one more time.

<em>Ex 2. Q3. What are the values in registers R0 and R1 after pressing play, but before pressing any other buttons?</em>

Then from there use the ‘Step in’ button. If you use the ‘Step over’ button you won’t be able to observe the recursion.

Just as in exercise 1, the register R1 will count down from 5 to 0 upon each invocation of the recursion. Once R1 has the value 0, it will stop recursing and finish executing the last call to the FACT subroutine. It stops because of the branch instruction in address x3205 which has the instruction ‘BRz BASE_3200. The condition code is finally zero upon the last decrement of R1 in the previous address.

Now continue pressing the ‘Step in’ button until you reach address x320E which has the instruction ‘LD R1, BACKUP_R1_3200’. From here, use only the ‘Step over’ button. This way you don’t have to go through the content of the MULT subroutine. This time, unlike last time, the return from this subroutine works. That’s what backing up R7 fixed from exercise 1.

Continue pressing ‘Step over’ until you reach the RET instruction. The program is about to return from the last recursive call.

<em>EX 2. Q4. What is the value of R7 before you execute the RET instruction?</em>

Now press ‘Step over’ and you should go back to the address from your answer above and execution will continue executing from there.

Continue pressing ‘Step over’ until the value in R0 is 1024.

<em>EX 2. Q5. Will this program ever finish, or does it just keep going?</em>

Now the program is stuck in a loop trying to return from the recursive subroutine. However, each time we return we keep overwriting R7 with the value where the recursive subroutine was called in the subroutine itself. It is never able to go back to where it was originally called in the main part of the program.

Once more, you’ll be expected to explain what happened that caused the program to not work correctly.

<u>Exercise 3</u>

For this final exercise we’ll fix the shortcomings from the last exercise by using a stack to backup and restore R7 and any other register we modify instead of a single memory location below the subroutine as in the previous exercises. In Lab 5 you were told to use the stack to back up the registers without understanding what a stack is, and without understanding why we need to use a stack. The last lab, Lab 6, taught you more about programming stack in assembly. This exercise will now illustrate why you need to use a stack, namely, to support recursion.

For this exercise, copy your code from lab 7 exercise 2, above, into the file lab7_ex3.asm. You’ll then add code to back up and restore the registers on the stack instead of memory locations at the end of each subroutine. But first you’ll need to set up the stack to be used throughout the program.

On the LC3 processor, we usually use R6 to store the top of the stack. In this case, we’ll use R5 to store the top of the stack since we’re using R6 to hold the subroutine address. This stack starts at memory location xFE00. You’ll need to modify the code from the previous exercise starting at address x3000. Change that code to look like the following:

<table width="40">
<tbody>
<tr>
<td width="40">1 2 3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20</td>
</tr>
</tbody>
</table>
;========================

; Main Program

;========================

.ORIG x3000

; Load stack

LD R5, STACK_ADDR

; Set R1 to 5

AND R1, R1, #0

ADD R1, R1, #5

; Call the factorial subroutine

LD R6, FACT_SUB_ADDR

JSRR R6

HALT

;========================

; Local Data

;========================

FACT_SUB_ADDR&nbsp;&nbsp; .FILL x3200

<table width="40">
<tbody>
<tr>
<td width="40">21 22</td>
</tr>
</tbody>
</table>
STACK_ADDR&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; .FILL xFE00

.END

All this additional code does is add a new label, STACK_ADDR, and load its value, xFE00 into R5. This initializes the stack, readying it for future calls to subroutines.

Next, change the beginning and end of each subroutine to use the stack instead of labels at the end of the subroutine. For example:

<table width="40">
<tbody>
<tr>
<td width="40">31 32 33

…

40 41 42
</td>
</tr>
</tbody>
</table>
ST R7, Save7_3100

ST R1, Save1_3100

; Subroutine code in between

LD R1, Save1_3100

LD R7, Save7_3100

Which backs up and restores R7 and R1 respectively, becomes:

<table width="40">
<tbody>
<tr>
<td width="40">31 32 33 34 35

…

42 43 44 45 46
</td>
</tr>
</tbody>
</table>
ADD R5, R5, #-1

STR R7, R5, #0

ADD R5, R5, #-1

STR R1, R5, #0

; Subroutine code in between

LDR R1, R5, #0

ADD R5, R5, #1

LDR R7, R5, #0

ADD R5, R5, #1

Which also backs up the same registers using the stack. Be sure to make this change for both the FACT and MUL subroutines. Also, pay close attention to the order in which you backup and restore the registers. When the registers are restored at the end of the subroutine, they should be restored in the <strong>reverse order </strong>in which they were backed up at the beginning of the subroutine. Also, be sure to do the subtractions and additions in the correct place. A common mistake is to do the addition when you’re restoring the values to the registers before the LDR. It should be after.

Once you’re done, assemble the code, put a breakpoint on the HALT instruction and run the program. Observe what happens. Did it work? (it should) See if you can figure out where the result of calling the FACT routine is stored.

<em>Ex 3. Q1. Which register holds the result of calling the FACT subroutine?</em>

<em>Ex 3. Q2. What value is stored in this register?</em>

<em>Ex 3. Q3. Is this the correct value for 5!?</em>

<h2>3.2&nbsp;&nbsp;&nbsp;&nbsp; Submission</h2>
Your TA will maintain a Google Sheet for questions and demos.

Demo your lab exercises to your TA <strong><em>before you leave the lab</em></strong>.

If you are unable to complete all exercises in the lab, demo the rest during office hours <strong><em><u>before </u></em>your next lab </strong>to get full credit. You can demo during the next lab with a 3 point deduction.

<em>Office hours are posted on Canvas (under Syllabus -&gt; Office Hours) and Discord (#office-hours).</em>
