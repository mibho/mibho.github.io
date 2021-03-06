---
layout: tocpost
title: denoobify x86 list
categories: [x86,x86-64]
excerpt: x86/x86-64 is .
---

<div class = "myWay">
    <p>
        x86/x86-64 can be .
    </p>
</div>

<details> 
    <summary> 
<h5> function prologue/epilogue </h5>
    </summary>
    <p>The function<a href=" .com">prologue prepares the stack for use by adjusting the appropriate registers as needed. </a> </p>
      <p> chek </p>
</details>
<br>
<br>
<br>


<details> 
    <summary> 
<h5> Visualizing the stack frame </h5>
    </summary>
    <p> The instructions are shown below (a specific portion from <code>sub_4010C0()</code>): <br>
    <img src="https://user-images.githubusercontent.com/86342821/142604889-85d5309e-7e98-4015-a365-612ea453fb04.png"> <br> <br>
          suppose our function's stack frame looks something like this, where EBP is x bytes away from ESP, as it's the base/start of that function's code. <br> 
<img src="https://user-images.githubusercontent.com/86342821/142606289-1b4d98d9-7d54-4c73-bab4-c16d56cec77b.png">
          After <code>add esp, 8</code> is executed, we have: <br>
<img src="https://user-images.githubusercontent.com/86342821/142606824-aa0a1d6b-5610-44a4-83e5-747c80309694.png"> <br> <br>
          then, there are two <code> push 0 </code>  <br>
        <img src="https://user-images.githubusercontent.com/86342821/142607146-ec614358-ab2e-40ab-b5b2-7354cabb292d.png"> <br>
         <img src="https://user-images.githubusercontent.com/86342821/142607543-a2038cdc-4511-4d2b-b838-a57561087e45.png"> <br> <br>
          The next instruction is: <code> mov ecx, [ebp+lpBuffer]</code>, which moves the contents of lpBuffer into ecx. Then <code> push ecx </code> is executed, resulting in: <br>
          <img src="https://user-images.githubusercontent.com/86342821/142612408-782a4c45-fa5e-4647-b9dd-7f4d9fc8c73a.png"> <br></p>
      <p> </p>
</details>
<br>
<br>
<br>

<details> 
    <summary> 
<h5> xor reg, reg </h5>
    </summary>
    <p>XOR <a href="https://www.pcmag.com/encyclopedia/term/xor">compares two separate bits and outputs one bit. </a> The result is 0 or 1 depending on whether or not the bits compared were the same. </p>
      <p>  </p>
</details>
<br>
<br>
<br>


<details> 
    <summary> 
<h5> LEA for quick multiplication </h5>
    </summary>
    <p>The function<a href=" .com">prologue prepares the stack for use by adjusting the appropriate registers as needed. </a> </p>
      <p> chek </p>
</details>
<br>
<br>
<br>


<details> 
    <summary> 
<h5> Use of PUSH instruction to allocate space for local variable(s)?  </h5>
    </summary>
    <p> In "normal" circumstances, if a register is PUSHed onto the stack, we can expect that it was done to either: save its current value so that it can be restored afterwards, or pass its contents along as an argument for a function. <br> </p>
      <p>However, there are instances in which the purpose of its usage might not be so obvious. Let's take a look at <a href="https://mibho.github.io/flarech2/">a function from my attempt of challenge 2 from 2021's Flareon8</a>. <br> </p>
</details>
<br>
<br>
<br>
  
  

    
    
  <details> 
    <summary> 
<h5> How does the PUSH/POP instruction affect ESP/RSP (stack pointer)? </h5>
  </summary>
      <p> do soon </p>
      <p> </p>
    </details>
    <br> 
    <br>
    <br>

