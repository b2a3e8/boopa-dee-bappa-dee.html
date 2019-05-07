<template>
  <div class="about">
    <h1 class="title">Boopa-Dee Bappa-Dee</h1>
    <p>Boopa-Dee Bappa-Dee is a programming language based on the vocabulary of <a target="_blank" href="https://www.youtube.com/watch?v=aS38wY1Fm34&feature=youtu.be">Peter Griffin's interpretation of the italian language</a>. It was invented .... TODO</p>
    <p>One could write entire programms in Boopa-Dee Bappa-Dee, however it's not very readable and effective.</p>
    <p>Actually Boopa-Dee Bappa-Dee is a brainfuck derivative. TODO...</p>
    <p>This Website...encode/decode.. TODO</p>

    <br />
    <table class="table">
      <thead>
        <tr>
          <th>Command</th>
          <th>Meaning</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td>bappadee</td>
          <td>increment the data pointer</td>
        </tr>
        <tr>
          <td>boo</td>
          <td>decrement the data pointer</td>
        </tr>
        <tr>
          <td>boopa</td>
          <td>increment the byte at the data pointer</td>
        </tr>
        <tr>
          <td>bappa</td>
          <td>decrement the byte at the data pointer</td>
        </tr>
        <tr>
          <td>dee</td>
          <td>output the byte at the data pointer</td>
        </tr>
        <tr>
          <td>beepee</td>
          <td>accept one byte of input, storing its value in the byte at the data pointer</td>
        </tr>
        <tr>
          <td>boopadee</td>
          <td>if pointer is zero, jump to matching baa</td>
        </tr>
        <tr>
          <td>baa</td>
          <td>if pointer is nonzero, jump to matching boopadee</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>
