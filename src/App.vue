<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<style lang="scss">
@import url('https://fonts.googleapis.com/css?family=Montserrat:700,600,500,400,300,100|Muli:300,400,500,600,700&display=swap');
*{
  margin:0;
  padding:0;
  box-sizing:border-box;
}

body {
    font-family:$font-family-muli;
    overflow-x:hidden;
    background: rgb(232, 245, 239);
}

h1, h2, h3, h4, h5,h6{
  font-family:$font-family-muli;
}

html, body, div, span, iframe,
  h1, h2, h3, h4, h5, h6, p, blockquote, pre,
  a, em, img,strong, i,ol, ul, li,
  fieldset, form, label, legend,
  table, caption, tbody, tfoot, thead, tr, th, td,
  article, aside, canvas, embed,
  figure, figcaption, footer, header, hgroup,
  nav, section,  audio, video {
      margin: 0;
      padding: 0;
      border: 0;
      vertical-align: baseline;
  }
  /* HTML5 display-role reset for older browsers */
  article, aside, details, figcaption, figure,
  footer, header, hgroup, nav, section {
      display: block;
  }
  input, button{
    font-family: $font-family-muli;
  }

  ol, ul{
      list-style: none;
  }

  table {
      border-collapse: collapse;
      border-spacing: 0;
  }
  a{
    color:#000;
    text-decoration:none;
  }

  .flex{
    display: -webkit-box;      /* OLD - iOS 6-, Safari 3.1-6 */
    display: -moz-box;         /* OLD - Firefox 19- (buggy but mostly works) */
    display: -ms-flexbox;      /* TWEENER - IE 10 */
    display: -webkit-flex;     /* NEW - Chrome */
    display: flex;
  }
  .flex--wrap{
    flex-wrap:wrap;
  }
  .flex-start {
    -webkit-justify-content:  flex-start;
      -moz-justify-content:  flex-start;
      -ms-justify-content:  flex-start;
      justify-content:  flex-start;

  }

  .flex-end {
    -webkit-justify-content:  flex-end;
      -moz-justify-content:  flex-end;
      -ms-justify-content:  flex-end;
      justify-content:  flex-end;
  }
  .text-center{
    text-align: center;
  }

  .column{
    -webkit-box-orient: vertical;
      -moz-box-orient: vertical;
    -o-box-orient: vertical;
      -ms-box-orient: vertical;

    -moz-flex-direction:column;
     -ms-flex-direction:column;
      -webkit-flex-direction:column;
       -o-flex-direction:column;
    flex-direction: column;
    width:100%;
  }
  .center {
    -webkit-justify-content: center;
      -moz-justify-content: center;
      -ms-justify-content: center;
      justify-content: center;
  }
  .middle{
    -webkit-align-items: center;
      -moz-align-items: center;
      -ms-align-items: center;
      -o-align-items: center;
      align-items: center;
  }
  .space-between {
    -webkit-justify-content: space-between;
      -moz-justify-content: space-between;
      -ms-justify-content: space-between;
      justify-content: space-between;
  }

  .space-around {
    -webkit-justify-content: space-around;
      -moz-justify-content: space-around;
      -ms-justify-content: space-around;
      justify-content: space-around;

  }


  .to-right{
    position:absolute;
    right:0;
    top:0;
  }

  .to-left{
    position:absolute;
    left:0;
    top:0;
  }
  .to-bottom{
    position:absolute;
    bottom:0;
  }
  .btn{
      display:inline-block;
      margin:5px;
      border-radius:50px;
      border:none;
      box-shadow: 0 2px 5px 0 rgba(0, 0,0, 0.12);
      transition: box-shadow 0.2s ease 0s, opacity 0.2s ease 0s;
      cursor:pointer;
      white-space: nowrap;
      font-family:$font-family-muli;
  }
  
  .color-white{
      color:#fff;
  }
  .no-shadow{
    box-shadow:none;
  }

  .text-center{
    text-align:center;
  }
  .text-right{
    text-align:right;
  }
  .text-left{
    text-align:left;
  }


  .col-s-20{
    width:20%;
  }
  .col-s-30{
    width:30%;
  }
  .col-s-33{
    width:33%;
  }
  .col-s-40{
    width:40%;
  }
  .col-s-50{
    width:50%;
  }
  .col-s-60{
    width:60%;
  }
  .col-s-70{
    width:70%;
  }
  .col-s-80{
    width:80%;
  }
  .col-s-100{
    width:100%;
  }

  .col-s-20, .col-s-30, .col-s-33, col-s-40{
    @include MQ($breakpoint-lg){
      width:50%;
    }
    @include MQ($breakpoint-sm){
      width:100%;
    }
  }
  .col-s-50, .col-s-60,.col-s-70, .col-s-80{
    @include MQ($breakpoint-md){
      width:100%;
    }
  }

</style>
