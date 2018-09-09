<template>
<div>
  <h1 class="terminal">
    <span class="path">{{ path }}</span><span>{{ msg }}</span>
  </h1>
</div>
</template>

<script>
export default {
  name: "Terminal",
  props: {
    msg: String,
    path: String
  }
};
</script>

<style scoped lang="scss">
div {
  display: inline-block;
  top: 50%;
  left: 50%;
  position: absolute;
  transform: translate(-51%, -50%);
}
.path {
  color: #e98da3;
}
.terminal {
  font-family: "Source Code Pro", monospace;
  font-weight: normal;
  overflow: hidden; /* Ensures the content is not revealed until the animation */
  border-right: 5px solid rgb(218, 218, 218); /* The typwriter cursor */
  white-space: nowrap; /* Keeps the content on a single line */
  margin: 0 0 auto; /* Gives that scrolling effect as the typing happens */
  letter-spacing: 0.15em; /* Adjust as needed */
  padding-right: 5px;
  -webkit-animation: blink-caret 0.75s step-end infinite;
  animation: blink-caret 0.75s step-end infinite;
}
</style>
